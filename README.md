<h1 style="color: #128c7e; font-weight: bold;">WAPY</h1>
<h2>WhatsApp Python Module</h2>

<p>Hi! I'm qq8 and im the developer of WAPY. Robby is my friend that sometimes help me with bugfixing or else, so i need to mention him too. WAPY is in the beta version so bugs may occur. If you get any errors or find bugs contact us at Discord qq8#3673, 32 rob#8637.
</p>

<h2>Usage</h2>

<p>The WhatsApp Python Module WAPY can be used to implement WhatsApp in your Python projects. Feel free and be creative! For example you can send specific output or variables from your Python projects to your friends on WhatsApp. Rise your business with a WhatsApp bot or just make an WhatsApp bot for you and your friends.</p>

<h2>Installation</h2>

**1.** Install WAPY and extract files in your project folder.

**2.** Install latest version of <a href="https://chromedriver.chromium.org/downloads" target="_blank">Chromedriver</a> and drag it into your project folder.

**3.** Install Selenium in cmd with <span style="color: green;">pip install selenium</span>.

**4.** Import wapy.py in your python file with <span style="color: plum">import</span> <span style="color: gray">wapy</span>.


Make sure your Python is up to date! WAPY was coded in **Python 3.8.6**, so if your Python version is to new or to old, there may occur errors or bugs.

<br>

> **Note:** WAPY was only tested on <a href=https://www.microsoft.com/windows target="_blank">Windows</a>.

<br>

<h2>Documentation</h2>

Here are listed all functions that are available in WAPY. 

<ul>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    init(driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Initialized WAPY.
    Firstly gets https://web.whatsapp.com. Secondly waits until QR-CODE is scanned.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    send(message, contact=None, driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Sends a message to specific contact or to focused contact.
    Add contact to send to specific contact.
    If no contact was given it will send message to focused contact.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    send_image(image, contact=None, driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Sends a image to specific contact or to focused contact.
    Add contact to send to specific contact.
    If no contact was given it will send image to focused contact.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    send_attachment(attachment, contact=None, driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Sends a attachment to specific contact or to focused contact.
    Add contact to send to specific contact.
    If no contact was given it will send attachment to focused contact.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    contact(contact, driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Opens chat of specific contact.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    contact_name(driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Gets the contact name of current open chat.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    refresh(driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Refreshes WhatsApp.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    message_in(message_index, driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Fetches a message from contact from open chat with given index.
    Index '-1' is last message.
    Messages contains 'type', 'text', 'image', 'time', 'author', 'element'.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    message_out(message_index, driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Fetches a message from yourself from open chat with given index.
    Index '-1' is last message.
    Messages contains 'type', 'text', 'image', 'time', 'author'.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    contact_presence(driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Gets the presence from open chat.
    Presence can be 'online', 'offline' or None if no chat is open.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    commandHandler(dictionary, index=-1, driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Responses on specific messages with specific message, image or attachment.
    Command handler runs only 1 time.
    <br>
    Command handler formation: '{command}': '{type}={text/path}'
    <br>
    {command} = a message to be replied to
    <br>
    {type} = 'text', 'image' or 'attach'
    <br>
    {text} = text message
    <br>
    {path} = path of file
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    response(command, response_type, text=None, path=None, index=-1, driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Responses on specific messages with specific message, image, attachment or returns 'True' boolean.
    <br>
    Response types are 'text', 'image', 'attach' or 'bool'.
    </span></li>
    <li style="margin-bottom: 20px"><span style="background-color: #242424; color: plum; padding: 3px;">
    unread(driver=driver)
    </span> = <span style="background-color: #242424; padding: 3px;">
    Checks if you got new message from contact.
    If you got new message from contact it will open chat from contact.
    </span></li>

</ul>

<h2>Examples</h2>

**1.** Easy response on specific message.

<pre>
import wapy

while True:
    unread()
    response('-wapy', 'text', text='Hello World!')

</pre>

<h3>Explanation</h3>
<p>Firstly we import wapy in out project folder with <span style="color: plum;">import wapy</span>. After that we code an <span style="color: plum;">while True</span> loop. A <span style="color: plum;">while True</span> loop runs the code in it forever. And we want that our WhatsApp Bot responses all the time, so we use it.</p>

<p>Inside the <span style="color: plum;">while True</span> loop we calling the function <span style="color: plum;">unread()</span>. That function checks all the time if you got a new message, and if you got a new message it opens the chat of the message author.</p>

<p>After we opened the chat of the message author we check if the message is '-wapy', and if it is we response with a text message. We are using the <span style="color: plum;">response()</span> function and giving the parameters <span style="color: plum;">response('-wapy', 'text', 'text='Hello World!')</span>.</p>

**2.** Advanced responses on specific messages.

<pre>
import wapy


with open('commands.json') as json_file:
    commands = json.load(json_file)

while True:
    commandHandler(commands)

</pre>

<h3>commands.json</h3>
<pre id="json">
{
    "-wapy": "text=WhatsApp Python automation. Developed by qq8 & robby.",
    "-version": "text=V.1.3"
}
</pre>

<h3>Explanation</h3>
<p>Firstly we import wapy in out project folder with <span style="color: plum;">import wapy</span>. After that we code an <span style="color: plum;">while True</span> loop. A <span style="color: plum;">while True</span> loop runs the code in it forever. And we want that our WhatsApp Bot responses all the time, so we use it.</p>

<p>After we imported wapy, we import our json file with:

<pre>
with open('commands.json') as json_file:
    commands = json.load(json_file)
</pre>

The json file must be formated as showed <a href="#json">above</a>.
</p>

<p>Inside the <span style="color: plum;">while True</span> loop we calling the function <span style="color: plum;">commandHandler()</span>. That function checks every command in the json file if it the message from your contact, and if it is, it responses with the given response in the json file.</p>

> **Note:** You also can use a dictionary instead of a json file.

<h2>Colors</h2>
WAPY is using the colors.py module. I made this module to print in colors.
<br>
<span style="color: white; font-weight: bold">!</span><span style="color: red; font-weight: bold"> DO NOT DELETE COLORS.PY OR WAPY WON'T WORK.</span>

<h2>Help</h2>
<p>If you need help, feel free to contact qq8#3673 or 32 rob#8637 on <a href="https://www.discord.com." target="_blank">Discord</a>.</p>
