# sdl-ui-kit
SDL2 C++ UI kit

Work In Progress

![license](https://i.creativecommons.org/l/by-nc-sa/2.0/88x31.png)

## Install

```
sudo apt-get install libsdl2-dev libsdl2-ttf-dev libsdl2-image-dev libboost-all-dev 
make
./main
```

## App

```
App app = App();
app.init(title, width, height, maximize);
app.setBackgroundColor(red, green, blue);
app.setWindowSize(width, height);
app.setTitle(title);
app.addWidget(widget);
app.addButton(button);
app.addText(text);
app.addTextbox(textbox);
app.addImage(image);
app.start();
```

## Widget

```
Widget widget1 = Widget(&app, x, y, width, height, red, green, blue);
widget1.setGeometryByPercentage(x, y, width, height);
widget1.setBorderWidth(int width);
widget1.setBorderColor(red, green, blue);
widget1.setColor(red, green, blue);
int w = widget1.getWidth();
int h = widget1.getHeight();
```

## Button

```
Button button1 = Button(&app, x, y, width, height, red, green, blue);
button1.cb = on_press_button1;
button1.setText(string text);
button1.setTextColor(red,green,blue);
button1.setFont(string font_path);
```

## Text

```
Text text1 = Text(&app, string text, x, y, width, height, red, green, blue);
text1.setText(string text);
text1.setTextColor(red, green, blue);
text1.setFont(string font_path);
```

## Textbox

```
Textbox textbox1 = Textbox(&app, string text, x, y, width, height, red, green, blue);
textbox1.setTextColor(red, green, blue);
textbox1.setFont(string font_path);
textbox1.setFontSize(int size);
```

## Image

```
Image image1 = Image(&app, "path/to/file.png", 0, 0, 30, 30);
```
