---
layout: chapter
bodyclass: chapter
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

      The Tkinter library provides a selection of widgets<br>
      we can use to build our apps.


      

##########


  - title: newproject
    class: centered-slide
    
    notes: |

      Create a new project

    content: |
      ## New Project

      Create a new project


##########


  - title: projectsettings
    class: centered-slide

    notes: |
      The pre-set settings should be fine, just check that the latest version of Python 3 is selected in the dropdown.

      You can also use these settings to change where your project will be saved on your computer.

    content: |

      ## Project Settings

      Choose where to save your project,<br>
      and the latest version of Python3


##########


  - title: appfile
    class: centered-slide

    notes: |

      Create a new file in your project. This will contain your app code, and will be the file we run to start up our app.

    content: |
      ## App Module

      Create a new file called `app.py`


##########


  - title: window
    class: centered-slide

    notes: |

      To get started creating our app, the first thing we need to do is import tkinter and create an app window.

      Importing tkinter allows us to create windows and also the widgets that we explore later.

      Calling the `mainloop` function starts your app running, and should always be done after setup.

    content: |
      
      ## Window

      Create a window for your app:

      ```language-python
      import tkinter
      window = tkinter.Tk()
      window.mainloop()
      ```

      You should see a window when you run your app.
      <!-- .element class="checkpoint" -->


##########


  - title: customwindow
    class: centered-slide

    notes: |

      The default window is 200 pixels square and has no title.

      We can customise our window a little using methods provided by tkinter.

    content: |
      ## Custom Window

      Customise your app window with additional options:

      ```language-python
      import tkinter
      window = tkinter.Tk()

      window.title("App of Awesomeness")
      window.geometry("300x300")

      window.mainloop()
      ```
      <!-- .element data-line="1-2, 7" -->

      Your window should now be bigger and have a title
      <!-- .element class="checkpoint" -->


##########


  - title: label
    class: centered-slide

    notes: |

      Let's explore some widgets available to us, starting with a simple label.

    content: |
      ## Label

      Create a label and add it to your window:

      ```language-python
      window.title("App of Awesomeness")
      window.geometry("300x300")

      label = tkinter.Label(window)
      label["text"] = "Hello"
      label.grid()

      window.mainloop()
      ```
      <!-- .element data-line="1-2, 8" -->

      Your window should now contain a label "Hello"
      <!-- .element class="checkpoint" -->


#########


  - title: button
    class: centered-slide
    
    notes: |

      We can also create buttons with ease.
    
    content: |
      ## Button
      
      Create a button and add it to your window:

      ```language-python
      label = tkinter.Label(window)
      label["text"] = "Hello"
      label.grid()

      button = tkinter.Button(window)
      button["text"] = "Click Me!"
      button.grid()

      window.mainloop()
      ```
      <!-- .element data-line="1-3, 9" -->

      Your window should now contain a button
      <!-- .element class="checkpoint" -->


##########


  - title: entry
    class: centered-slide

    notes: |

      Creating text inputs can be done using the Entry widget.

    content: |
      ## Entry

      Add a text entry box to your window:

      ```language-python
      button = tkinter.Button(window)
      button["text"] = "Click Me!"
      button.grid()

      entry = tkinter.Entry(window)
      entry.grid()

      window.mainloop()
      ```
      <!-- .element data-line="1-3, 8" -->

      Your window should now contain a text entry area
      <!-- .element class="checkpoint" -->


##########

  - title: listbox
    class: centered-slide

    notes: |

      You may also have need of a list box

    content: |

      ## Listbox

      Add a list box to your app:

      ```language-python
      entry = tkinter.Entry(window)
      entry.grid()

      listbox = tkinter.Listbox(window)
      listbox.grid()

      window.mainloop()
      ```
      <!-- .element data-line="1-2, 7" -->

      Your window should now contain a list box
      <!-- .element class="checkpoint" -->


##########


  - title: challenge
    notes: |

      You will need the widgets we have covered, and also some that we have not.

    content: |

      ## Challenge:<br> Application Form
      
      ![Cat App Example]([[BASE_URL]]/media/images/slidecontent/cat-app.png)
      <!-- .element height="445" -->

      Recreate this app using what you have learned.

      


##########


  - title: summary
    class: centered-slide

    notes: |

      Great! That's the basics out of the way, now let's move on to layouts.

    content: |

      ![Thumbs Up!]([[BASE_URL]]/assets/images/thumbs-up.svg)
      <!-- .element height="200" -->

      ## Graphical Widgets: Complete!

      Great, now let's do some more complex layouts...

      [Take me to the next chapter!](layouts.html)


---


<section class="container content-panel">

## App Window


### Basic Example

```python
window = tkinter.Tk()
window.mainloop()
```

### Complex Example

```python
window = tkinter.Tk()

window.title("App of Awesomeness")
window.geometry(300, 300)

window.mainloop()
```

### Properties

None of note


### Functions

- mainloop
- title
- geometry

</section>


<section class="container content-panel">

## Label

### Basic Example

```python
my_label = tkinter.Label(app_window)
my_label["text"] = "Hello!"
my_label.grid()
```

### Complex Example

```python
my_label = tkinter.Label(app_window)
my_label["text"] = "Hello!"
my_label["fg"] = "red"
my_label["font"] = "Comic Sans MS", 16, "bold"
my_label.grid()
```

### Properties

- **text** <br> The words to display on the label.
- **fg** <br> The text colour. The letters "fg" stand for "foreground".
- **font** <br> Font properties including the actual font, size in pixels, and whether it should be bold or italic.

### Functions

None of note

</section>



<section class="container content-panel">

## Entry

### Basic Example

```python

```

### Complex Example

```python

```

### Properties

None of note

### Functions

None of note

</section>



<section class="container content-panel">

## Text

### Basic Example

```python

```

### Complex Example

```python

```

### Properties

None of note

### Functions

None of note

</section>



<section class="container content-panel">

## Button

### Basic Example

```python

```

### Complex Example

```python

```

### Properties

None of note

### Functions

None of note

</section>



<section class="container content-panel">

## Listbox

### Basic Example

```python

```

### Complex Example

```python

```

### Properties

None of note

### Functions

None of note

</section>
