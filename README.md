# Smart-thermostat
This project is the smart thermostat-based fault correction strategies

In this project, we employed the two-way OpenAPI functionality provided by the thermostat product to develop self correction algorithms. The algorithms include inefficient HVAC setpoints, schedules, and deadbands, which have been tested using EMIS tools.  
The scripts include three major scripts as: 1) pelican_openapi_io_driver.py; 2) func_schedule_fault_detection_correction.py, and 3) func_setpoint_setting_fdd_correction.py
pelican_openapi_io_driver.py is the main script, which interfaces with the Pelican cloud to pull data and write back data. In addition, it calls the FDD and correction algorithms.
func_schedule_fault_detection_correction.py includes the schedule fault detection and correction algorithms.  
func_setpoint_setting_fdd_correction.py includes the setpoint setting fault detection and correction algorithms (including cooling setpoint too low, heating setpoint too high, and narrow deadband).

One data .csv file (hist_data_2023-06-15_2023-07-12.csv) can be used to test and debug the algorithms. 
