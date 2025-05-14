This was a project to implement a simple client side editor. 

The project uses codemirror v5 to implement a javascript editor in a browser. 

The implementation uses codemirror directly, so you don't need to import or do any npm setup.

To have this running do:
`git clone` and open the `index.html` file from the local clone.

You should see something along the lines of the following screenshot in your browser

![basic-functionality](https://github.com/user-attachments/assets/094d29d6-5337-48bd-9c68-5de284babe13)


Two nice features that are demonstrated are traditional intellisense and a custom intellisense autocomplete.

![ctrl-q-intellisense](https://github.com/user-attachments/assets/60bc8302-ac2a-4e7f-9fda-a21afa398e98)

This feature is provided by codemirror but you need to configure it with the hint addons. 

The custom autocomplete provides whatever you use, I have it using only a couple of basic commands, a templated for loop, a `let` and a `const` declaration. 

![ctrl-e-custom-autocompletes](https://github.com/user-attachments/assets/5ef0664f-6be0-4617-bab3-26b9f0601569)

These are more for illustration purposes than what you would actually want in practice.

In the screenshots you'll also notice a `browse` button and a `download` button. 

For the `browse` button you can select a file from the local filesystem and import that as a started code if you wanted but it isn't required. 

For the `download` button you can download the current contents of the editor into a filename which you provide in the form. 
I prepopulate with the value `MyMirrorFile.js` but you could make it whatever you wanted and it will download to your downloads folder.

I tested the use of this in firefox browser and chrome, it works in both. 
