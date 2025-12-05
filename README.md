# porkbun_ddns_bash
Porkbun Dynamic DNS Linux Bash Script

This allows you to update a porkbun dns server with updated info.  The script can be run every 5 minutes if you like because it saves the last public ip address. It does hit api.ipify.org every time though, so it is best to keep it reasonable. If the ip address is updated (or the currentip file is removed), it will read your current DNS setting to see if it has changed.  If it has changed, it will update the dns entry.  Once finished successfully, it updates the last ip file so that future runs of the script minimize api calls.
