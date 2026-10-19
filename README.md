# BDMV-Template-for-Simple-Xlets
A ready-to-use BDMV directory template for making and testing simple BD-J Xlets.

# What’s inside the ZIP
- Full BDMV directory (including CERTIFICATE folder)
- SOURCE directory containing
    - Hello World `Xlet.java`
    - `.perm` file
    - `BD-J.jar` (needed for compilation)
# Instructions
1. Download and install Java 8 JDK (Adoptium Temurin 8 is recommended). Newer Java versions are not recommended.
2. Download the template ZIP and extract it.
3. Create three folders on your desktop:
    - `BDJProject` ← put the SOURCE folder contents here
    - `BDJProjectBDMV` ← put the BDMV folder here
    - `ISO Output`
4. Compile the Xlet: Double-click `BuildXlet.bat` inside the `BDJProject` folder. It will compile the Java file into `.class` files using Java 1.3 compatibility.
5. Package into a JAR: Open Command Prompt and run these commands one by one:
  - ```cd C:\Users\YOURNAME\Desktop\BDJProject```
  - ```jar cvf 00000.jar -C src .```
6. Copy the newly created `00000.jar` into:
- ```BDJProjectBDMV\BDMV\JAR\```
7. Create the ISO with ImgBurn:
    - Open ImgBurn → Create image file from files/folders
    - Select the BDJProjectBDMV folder as source
    - Save the ISO into your ISO Output folder
    - Accept the default volume label and “BD Video” detection
8. Test the ISO in VLC, PowerDVD, a Dune HD, or burn it to a BD-RE disc.


# Important Notes
- Do not modify the MovieObject.bdmv, Index.bdmv, BDJO file, or .perm file when making simple single-Xlet projects.
- The BD-J.jar is required by BuildXlet.bat to compile to Java 1.3 bytecode.




 
