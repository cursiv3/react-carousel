Simple photo carousel React component. 

To install: 

npm i --save corousel

- Place photo URLs or paths into an array and pass it
to the `images` prop on the Carousel component:

```
    import Carousel from "corousel";
    
    var pictures = [
        './somepath/toPic.jpg',
        'https://www.myphotourl.com/thisPic',
        'https://www.myphotourl.com/thisPic2'
    ];

    <Carousel images={pictures} />
```



- Default width/height are set to 100%.
- Change that using the height or width props:

```
    <Carousel images={pictures} height={'300px'} width={'70%'} />
    ...
    <Carousel images={pictures} width={'1500px'} />
    ...
    <Carousel images={pictures} height={'600px'} />
    ...
    <Carousel images={pictures} height={'50%'} width={1500} />
    //etc
```

- The "legend" defaults to dots 
- If picture array is larger than 15 it changes to a number display in the bottom right corner.
- Change to number legend by using the ```legend``` prop on the component and setting
it to the string "numbers":

```
    <Carousel images={pcitures} legend={"numbers"} />

    // any other value given to legend is ignored and the dots are shown
```


Simple and I hope lightweight and easy to use.  I plan on updating and giving an
api to control slide speed, image fadein/out amount and speed, button size, and
an autoplay.  Stay tuned!
