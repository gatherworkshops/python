---
layout: chapter
title: Graphical Widgets
course: levelthree

slides:

  - title: title-page
    class: title-slide

    notes: |

      To create a GUI or Graphical User Interface, we can use a set of ready-made widgets which come with Python.

      These widgets can be combined in any layout to create a basic app.

    content: |

      ![Gather Workshops Logo]([[BASE_URL]]/assets/images/gw_logo.png)

      # Graphical Widgets
      _The components that make up apps_


##########

  - title: tkwidgets
    layout: centered-slide

    notes: |

      We will be using a widget library called Tkinter. 

      The set of widgets available to us isn't large, but we can achieve most basic apps with the options available.

    content: |

      ## TkInter Widgets


      

##########


  - title:
    content: |
      ## New Project


  - content: |
      ## Project Settings


  - content: |
      ## App Module (app.py)


  - content: |
      ## Window

      ```language-python
      import tkinter
      window = tkinter.Tk()
      window.mainloop()
      ```


  - content: |
      ## Custom Window

      ```language-python
      import tkinter
      window = tkinter.Tk()

      window.title("App of Awesomeness")
      window.geometry("300x300")
      window.wm_iconbitmap("appname.ico")

      window.mainloop()
      ```
      <!-- .element data-line="4-6" -->


  - content: |
      ## Label

      ```language-python
      label = tkinter.Label(window)
      label["text"] = "Hello"
      label.pack()
      ```


  - content: |
      ## Button
      
      ```language-python
      button = tkinter.Button(window)
      button["text"] = "Click Me!"
      button.pack()


  - content: |
      ## Entry

      ```language-python
      entry = tkinter.Entry(window)
      entry.pack()
      ```


  - content: |
      ## Challenge

      Reproduce the example UI


  - title: summary
    class: centered-slide

    notes: |

      Great! Now that's all sorted, let's get started!

    content: |

      ![Thumbs Up!]([[BASE_URL]]/assets/images/thumbs-up.svg)
      <!-- .element height="200" -->

      ## Graphical Interfaces: Complete!

      Great, now it's time for the fun stuff...

      [Take me to the next chapter!](layouts.html)


---