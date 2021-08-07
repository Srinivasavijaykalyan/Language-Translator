# Language Translator
Tkinter Programming
Tkinter is the standard GUI library for Python. Python when combined with Tkinter provides a fast and easy way to create GUI applications. Tkinter provides a powerful object-oriented interface to the Tk GUI toolkit.
Tkinter is a Python Package for creating GUI applications. Python has a lot of GUI frameworks, but Tkinter is the only framework that's built into the Python standard library. Tkinter has several strengths; it's cross-platform, so the same code works on Windows, macOS, and Linux
from tkinter import *

import tkinter as tk
from tkinter import ttk
from PIL import ImageTk, Image
from googletrans import Translator
from tkinter import messagebox



l = tk.StringVar() 
choose_langauge = ttk.Combobox(root, width = 20, textvariable = l, state='readonly',font=('verdana',10,'bold')) 

There are many languages in the translator (approx 100), These are the languages that can be translated by using this Project Language Translatoor
  


choose_langauge['values'] = (
                        'Afrikaans',
                        'Albanian',
                        'Arabic',
                        'Armenian',
                       ' Azerbaijani',
                        'Basque',
                        'Belarusian',
                        'Bengali',
                        'Bosnian',
                        'Bulgarian',
                       ' Catalan',
                        'Cebuano',
                        'Chichewa',
                        'Chinese',
                        'Corsican',
                        'Croatian',
                       ' Czech',
                        'Danish',
                        'Dutch',
                        'English',
                        'Esperanto',
                        'Estonian',
                        'Filipino',
                        'Finnish',
                        'French',
                        'Frisian',
                        'Galician',
                        'Georgian',
                        'German',
                        'Greek',
                        'Gujarati',
                        'Haitian Creole',
                        'Hausa',
                        'Hawaiian',
                        'Hebrew',
                        'Hindi',
                        'Hmong',
                        'Hungarian',
                        'Icelandic',
                        'Igbo',
                        'Indonesian',
                        'Irish',
                        'Italian',
                        'Japanese',
                        'Javanese',
                        'Kannada',
                        'Kazakh',
                        'Khmer',
                        'Kinyarwanda',
                        'Korean',
                        'Kurdish',
                        'Kyrgyz',
                        'Lao',
                        'Latin',
                        'Latvian',
                        'Lithuanian',
                        'Luxembourgish',
                        'Macedonian',
                        'Malagasy',
                        'Malay',
                        'Malayalam',
                        'Maltese',
                        'Maori',
                        'Marathi',
                        'Mongolian',
                        'Myanmar',
                        'Nepali',
                        'Norwegian'
                        'Odia',
                        'Pashto',
                        'Persian',
                        'Polish',
                        'Portuguese',
                        'Punjabi',
                        'Romanian',
                        'Russian',
                        'Samoan',
                        'Scots Gaelic',
                        'Serbian',
                        'Sesotho',
                        'Shona',
                        'Sindhi',
                        'Sinhala',
                        'Slovak',
                        'Slovenian',
                        'Somali',
                        'Spanish',
                        'Sundanese',
                        'Swahili',
                        'Swedish',
                        'Tajik',
                        'Tamil',
                        'Tatar',
                        'Telugu',
                        'Thai',
                        'Turkish',
                        'Turkmen',
                        'Ukrainian',
                        'Urdu',
                        'Uyghur',
                        'Uzbek',
                        'Vietnamese',
                        'Welsh',
                        'Xhosa'
                        'Yiddish',
                        'Yoruba',
                        'Zulu',
                          ) 
  
choose_langauge.place(x=290,y=70)
choose_langauge.current(0) 


t1 = Text(root,width=30,height=10,borderwidth=5,relief=RIDGE)
t1.place(x=10,y=100)

t2 = Text(root,width=30,height=10,borderwidth=5,relief=RIDGE)
t2.place(x=260,y=100)


button = Button(root,text="Translate",relief=RIDGE,borderwidth=3,font=('verdana',10,'bold'),cursor="hand2",command=translate)
button.place(x=150,y=280)


clear = Button(root,text="Clear",relief=RIDGE,borderwidth=3,font=('verdana',10,'bold'),cursor="hand2",command=clear)
clear.place(x=280,y=280)

root.mainloop()
