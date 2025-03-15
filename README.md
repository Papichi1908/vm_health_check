# VM Health Check

This repository contains a shell script to analyze the health of an Ubuntu virtual machine based on CPU, memory, and disk space utilization.

## Script Details
The script checks the following parameters:
- **CPU Utilization**: The percentage of CPU being used.
- **Memory Utilization**: The percentage of memory being used.
- **Disk Space Utilization**: The percentage of disk space being used.

If any of these parameters are more than 60% utilized, the script declares the state as "Not healthy". Otherwise, it declares the state as "Healthy".

## Usage
1. Save the script to a file named `vm_health_check.sh`.
2. Make the script executable with the command:
   ```bash
   chmod +x vm_health_check.sh
   ```
3. Run the script to check the health status:
   ```bash
   ./vm_health_check.sh
   ```
4. Run the script with the `explain` argument to get detailed reasons for the health status:
   ```bash
   ./vm_health_check.sh explain
   ```

## Example
To check the health status of the virtual machine:
```bash
./vm_health_check.sh
```

To check the health status with explanations:
```bash
./vm_health_check.sh explain
```

## License
This repository is licensed under the MIT License.
