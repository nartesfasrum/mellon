# Mellon (pfSense Captive Portal + MQTT Integration)

## Setup Instructions

These instructions assume you have a captive portal and vouchers already set up.

Note: you must ensure the names of the provided files do not change, or styling will break. When you upload files to the pfSense captive portal under the "File Manager" tab, the file manager appends 'captiveportal-' to the filename. This is fine, & the pages have the appropriate links to accomodate this.

- Change the values in welcome.html as appropriate to match your MQTT configuration
- Open the captive portal configuration for the appropriate captive portal zone
- Set the "After authentication Redirection URL" to http://[captive portal URL]/captiveportal-welcome.html
- - ex. for a captive portal running at 10.0.20.1, the URL will look like http://10.0.20.1:8002/captiveportal-welcome.html
- Enable the "Use custom captive portal page" option
- Upload voucher.html under the "Portal page contents" option
- Save your configuration changes
- Under the "File Manager" tab of the captive portal configuration, upload styles.css and welcome.html

## License

Copyright 2021 Nikolai Mallett.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
