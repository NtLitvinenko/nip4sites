# NIP Markup File (nipmf = nmf)
# This is comment btw.
# markuptype_Varname:style
# style_Stylename:styles like
# style_Button1:{bgcolor=red;text=Click me!;x=10;y=10}
# remove spaces if needed
style_Button1:{bgcolor=red;text=Click me!;x=10;y=10}
style_Label1:{text=Hi, world!;x=50;y=50}
style_btn:{text=Button clicked!!!;background=black;foreground=white;x=255;y=255}
label_Hello:style_Label1
button_Button:style_Button1
button_Button.onclick:function_OnButtonClick
function_OnButtonClick{
    label_Label1=style_NewStyle
    exec:print?Hello World[?]
    exec:destroy?label_Hello
    exec:createWidget?label_Hi?style_btn
}
