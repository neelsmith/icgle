
Use LICECap to grab screen as gif.

Trim away excess frames in Preview.

If this hoses looping, use image magick to fix it:


    convert -loop 0 screenie-mod.gif looper.gif