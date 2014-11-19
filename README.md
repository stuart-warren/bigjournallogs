BigJournalLogs
==============

Testing that the SystemD journal is capable of handling large log lines

```
wget https://github.com/stuart-warren/bigjournallogs/releases/download/0.1/bigjournallogs
chmod +x bigjournallogs
./bigjournallogs
journalctl -b | grep bigjournallogs
```

Should show the full message in a single log entry, not split at the 2048th character.
