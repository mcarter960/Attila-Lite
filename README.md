# Attila Lite Theme

A content focused responsive theme for [Ghost](https://github.com/tryghost/ghost/). See a demo at: [http://attila-lite.devops10.com/](http://attila-lite.devops10.com/)

I forked this project from https://github.com/zutrinken/attila Peter Amende is the Author.

The reason I did was to retain the Light Theme in the original release.

I am NOT a developer, just changing a few settings here and there. Peter has helped me via email correspondence and I am very grateful!

#I am NOT changing any of Peters Code, just sass/style.css to retain light colors.



## Screenshots

<table>
<tr>
<td valign="top">
<img src="https://raw.githubusercontent.com/zutrinken/attila/master/src/screenshot-desktop.jpg" />
</td>
<td valign="top">
<img src="https://raw.githubusercontent.com/zutrinken/attila/master/src/screenshot-mobile.jpg" />
</td>
</tr>
</table>

## Features

* Responsive layout
* Dark Mode
* Search
* Post reading progress
* Code highlight including line numbers
* Disqus support

## Localization

* __English__
* __German__
* __Spanish__
* __French__ by [robink](https://github.com/robink)
* __Italian__ by [fmaida](https://github.com/fmaida)
* __Norwegian__ by [arthurnoerve](https://github.com/arthurnoerve)
* __Chinese__ by [hao-lee](https://github.com/hao-lee)
* __Indonesian__ by [simplyeazy](https://github.com/simplyeazy)
* __Romanian__ by [cdorin93](https://github.com/cdorin93)
* __Russian__ by [schamberg97](https://github.com/schamberg97)
* __Turkish__ by [cgrgrbz](https://github.com/cgrgrbz)

## Setup [Disqus](https://disqus.com/)

1. Go to __Code injection__.  
2. Add this to __Blog Header__:  
````
<script>var disqus = 'YOUR_DISQUS_SHORTNAME';</script>
````

## Setup search

The search function is build with [ghostHunter](https://github.com/jamalneufeld/ghostHunter):

1. Go to __Integrations__.  
2. Choose __Add custom integration__, name it `ghostHunter` and choose __Create__. Copy the generated Content API Key.  
3. Go to __Code injection__.  
4. Add this to __Blog Header__:  
````
<script>
  var ghosthunter_key = 'PASTE_THE_GENERATED_KEY_HERE';
  //optional: set your custom ghost_root url, default is "/ghost/api/v2"
  var ghost_root_url = '/ghost/api/v2';
</script>
````
## Development

Install [Node-Sass](https://www.npmjs.com/package/node-sass):

	npm install node-sass

Install [Grunt](https://gruntjs.com/getting-started/):

	npm install -g grunt-cli

Install Grunt dependencies:

	npm install

Build Grunt project:

	grunt build

The compress Grunt task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

	grunt compress

## Command line Output
```
~/Attila-Lite$ sudo npm install node-sass
npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142

> node-sass@4.13.1 install /home/ghostadmin/Attila-Lite/node_modules/node-sass
> node scripts/install.js

Cached binary found at /home/ghostadmin/.npm/node-sass/4.13.1/linux-x64-64_binding.node

> node-sass@4.13.1 postinstall /home/ghostadmin/Attila-Lite/node_modules/node-sass
> node scripts/build.js

Binary found at /home/ghostadmin/Attila-Lite/node_modules/node-sass/vendor/linux-x64-64/binding.node
Testing binary
Binary is fine
+ node-sass@4.13.1
added 84 packages from 105 contributors and audited 1728 packages in 14.185s

1 package is looking for funding
  run `npm fund` for details

found 0 vulnerabilities

~/Attila-Lite$ sudo npm install -g grunt-cli
/usr/bin/grunt -> /usr/lib/node_modules/grunt-cli/bin/grunt
+ grunt-cli@1.3.2
updated 1 package in 5.299s
~/Attila-Lite$ sudo npm install
audited 1728 packages in 2.622s

1 package is looking for funding
  run `npm fund` for details

found 0 vulnerabilities

~/Attila-Lite$ sudo grunt build
Running "sass:dist" (sass) task

Running "postcss:dist" (postcss) task
>> 1 processed stylesheet created.

Running "copy:dist" (copy) task
Copied 5 files

Running "uglify:js" (uglify) task
>> 1 file created 268.99 kB → 186.51 kB

Done.
~/Attila-Lite$ sudo grunt compress
Running "compress:main" (compress) task
>> Compressed 1 file

Done.
~/Attila-Lite$ ls -lt dist/
total 828
-rw-r--r-- 1 root root 847757 Mar  2 00:32 attila-lite.zip
```

## Copyright & License

From Peter's GitHub Page: Copyright (C) 2015-2020 Peter Amende - Released under the [MIT License](https://github.com/zutrinken/attila/blob/master/LICENSE).

Copyright (C) 2015-2020 Arthur Carter - Released under the [MIT License](https://github.com/mcarter960/Attila-Lite/blob/master/LICENSE).
