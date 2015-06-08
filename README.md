

Microsoft Internet Explorer 9




interoperabilitybridges.com   


 

INSTALLATION / UNINSTALLATION 

To install:
     Unzip the IE9FileAPI.zip file in a directory of your choice

Run the following commands from an elevated command prompt. 
 (For instructions on opening an elevated command prompt, see: http://windows.microsoft.com/en-US/windows7/Command-Prompt-frequently-asked-questions)
     cd "[path where files were unpacked into]"
     regsvr32.exe fileapi.dll 

To uninstall, close all running instances of Microsoft Internet Explorer and run the following commands from an elevated command prompt window: 
     cd "[path where files were unpacked into]"
     regsvr32.exe /u fileapi.dll 

GETTING STARTED 

1.Launch "File API Samples.html" in your IE browser. 

1.1.You will see the browser warning: "Internet Explorer restricted this webpage from running scripts or ActiveX controls" above the browser status bar. 

1.2.Click on "Allow Blocked Content". 

2. Click on the buttons on the page to exercise the corresponding Scenarios

KNOWN LIMITATIONS AND DIFFERENCES FROM DRAFT 

In this implementation:

1.The methods readAsBinaryString(), and readAsArrayBuffer() in the FileReader interface are not supported

2.The FileReaderSync interface is not supported

3.Error Handling and Exceptions differ from the Draft

4.Note that this sample provides helper bootFileAPI.js script, which allows access to the draft File API using "new FileReaderDraft()", "window.URLDraft", and "GetFileSelector" syntax. This is due to the fact that the functionality is currently provided via plugin as opposed to natively in IE9.

5.This release has modified the slice method to match the new File API spec, released April 19, 2011.

6.In this release we added a sample to read multiple files.

FEEDBACK 

Microsoft welcomes feedback on this implementation. Please send your thoughts to HTML5_FILEAPI@mailinglist.interoperabilitybridges.com
