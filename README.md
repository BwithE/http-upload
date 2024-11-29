# http-upload
![image](https://github.com/user-attachments/assets/6fcfbe34-4a3d-43b0-a280-b97082cedab7)

A Python HTTP server that runs on port 80 and receives files from remote machines.

They will be uploaded into the current working directory that it's ran.

It's an easy way to trasfer files without the need of SSH and compromising usernames.

The webpage has buttons that can be used, however, below is a list of CLI commands to get the job done.

Windows clients need `curl.exe` which can be found at "https://curl.se/windows/"

# USAGE
`python3 upload-server.py`


# CLIENT USAGE
- WINDOWS POWERSHELL UPLOAD COMMAND
	- `curl -X POST -F "file=@c:\path\to\your\file.txt" http://<PYTHON_SERVER_IP>`

- LINUX UPLOAD COMMAND
	- `curl -X POST -F "file=@/path/to/your/file.txt" http://<PYTHON_SERVER_IP>`
