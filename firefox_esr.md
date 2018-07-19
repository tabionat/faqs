# Install procedure for Firefox ESR + Java Web Start Apps

Manually install Firefox ESR
* https://www.mozilla.org/en-US/firefox/organizations/all/#legacy
* install to /usr/lib/firefox_esr
* sudo ln -s /usr/lib/fireforx_esr /usr/bin/firefox_esr

Install Java runtime environment:
* https://java.com/en/download/manual.jsp#lin (could be a differnet version)
* last installed version jre1.8.0_171
* install to /usr/local/java/jre1.8.0_171

Run Firefox ESR once to seed config directories in ~/

Add plugin soflink:
* 32-bit version: sudo ln -s /usr/local/java/jre1.8.0_171/lib/i386/libnpjp2.so ~/.mozilla/plugins
* 64-bit version: sudo ln -s /usr/local/java/jre1.8.0_171/lib/amd64/libnpjp2.so ~/.mozilla/plugins
* See https://docs.oracle.com/javase/8/docs/technotes/guides/install/linux_plugin.html for more details

Test Java at https://www.java.com/en/download/installed.jsp

