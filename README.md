
## What's PSD2HTML?

Just as the name says, PSD2HTML is a tool to generate a static html page along with the image resources required from Photoshop PSD file.   

## What's the Difference Between PSD2HTML and PS's Build-in Html Export Functionality?

Photoshop has a build-in html export functionality, but the main problem is that we cann't edit the output html file's text, not to say the font-styles, etc. All The texts are parts of the image file. It's quite inconvenient for web page editors.<br/>
However, PSD2HTML cope with this situation much better. **The images and texts are seperated!** As a matter of fact, if the font been used is listed in PSD2HTML/lib/web-fonts.jsx, then the texts will be seperated, or the texts will be parts of the image file.<br/>

## Usage:
**The PS plugin version can be installed this way:<br/>**
- Copy PSD2HTML directory and PSD2HTML.jsx to (PS installation directory)\Presets\Scripts\ <br/>
- Restart Photoshop<br/>
- Open the psd file you want to process, choose PSD TO HTML menu item in Help menu. And the plugin will do the rest for you. All the Html and image files will be generated. <br/>

**There is also a Node Version Html Generator:<br/>**
- To generate html pages by node server, you should upload the *.txt and *.png files generated by this plugin, and the server will generate the html file and image slices required, pack all the resources up, finally, provide a download link. For more information, see the readme file in server directory.

------------------------

##PSD TO HTML为Photoshop插件，运行该插件将会对当前PSD文件进行解析，然后生成HTML文件及图片。  

###该插件分为两个版本
####PS版：  
此版本将解析PSD文件，然后输出HTML文件及图片到你指定的文件夹。

####Nodejs版：
此版本先利用该插件生成一个TXT文件和一张PNG图片，然后将TXT文件和PNG图片上传至服务器，服务器生成HTML文件和图片文件提供下载。

####安装及使用方法：
1、将PSD2HTML文件夹及PSD2HTML.jsx复制到Photoshop安装目录的\Presets\Scripts下  
2、重启Photoshop  
3、打开PSD文件，点击Photoshop的帮助菜单下的PSD TO HTML菜单  