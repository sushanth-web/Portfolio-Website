1.create a package.json by using command npm init in powershell of the folder give the details and click enter you will have a package.json file

2.Install the packages we need DART-SASS(a type of sass), BOOTSTRAP 5(css framework),FONTAWESOME(for icons),AUTOPREFIXER(adds styles for css so it runs on all browsers and older versions)

3.command to install dart sass type in terminal(powershell) of folder you wanna install in 'npm install --save-dev sass'  after installation is complete you will see a new folders called as nodemodules,package-lock.json

4.to install bootstrap go to the website getbootstrap.com and copy the command 'npm install bootstrap@5.3.6 --save' and use it in terminal to install

5.to install fontawesome use the command  'npm install --save @fortawesome/fontawesome-free'

6.to install autoprefixer use command 'npm install postcss-cli autoprefixer --save'

7.go to package.json remove the text inside scripts and replace it with "compile:sass":"sass --watch scss:assets/css" what it does is creates a function with name compile:sass and what it does is compiles sass from scss folder to css and saves it in assets folder under css folder and also watches all the sass files in scss folder, to make it active after saving the scripts in package.json file run the command 'npm run compile:sass' in terminal which tells the terminal to run the function compile:sass after the command we will get a new folder called assets which contains a folder css and the css will have compile css files from scss folder. the css folder will have two files one is .css and one is .css.map this file is called as sorce maps they make it possible to edit your sass files in browser when we inspect.

8.the css is generated only when the terminal is watching the sass files so make sure it watches the sass files by using the command 'npm run compile:sass'  before seeing the output 

9.//IMPORTING BOOTSTRAP 5
@import "../node_modules/bootstrap/scss/bootstrap.scss"; in _custom.scss

10.@use 'custom'; in style.scss and save both now you can see all the bootstrap variables been compiled to style.css

11.we can copy icons from bootstrap website directly by going to icons section and search for your favourite icon and paste it in your code

12.we downloaded bootstrap javascript sourcefiles from the website and moved the js folder to assets folder

13.we copied the navbar from bootstrap website bootstrap website -> docs -> components ->nav bar->look for different navbars and find the one you want and copy code and paste it in html

14.we copied webfonts folder from node_modules->@fontawesome->fontawesome-free->webfonts  to assets folder

15.we are getting the image from many pixels website

16.this is the wave we got from the website getwaves.io change the fill=#fff" to your favourite color

17.we install glightbox to display video when we click play button glightbox supports all screensnpm install glightbox
we installed it from github and pasted css,js folders from dist of glighthub we installed from github into newly created
vendors folder in assets

18.<script type="text/javascript">

  const lightbox = GLightbox({
    'href': 'https://youtu.be/jS4aFq5-91M?si=EcVQ1KIIzrNz324E',
    'type': 'video',
    'source': 'youtube', //vimeo, youtube or local
    'width': 900,
    'autoPlayVideos':'true',
});

</script>
we added this code at bottom and added a class glightbox to the link we want video to popup to

we are getting the footer icons from tablericons.com