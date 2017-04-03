# Sync time via NTP for every 5 minutes 

This is to create crontab scripts that will sync time to NTP every 5 minutes. This is crucial for VM (ie Virtualbox) that is not shutdown properly or paused from time to time.

```
# crontab -u root -l
*/5 * * * * /usr/sbin/ntpdate -s time.nist.gov
```