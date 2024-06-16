
# How I Use the Daily Notes Plugin: A Comprehensive Guide
A comprehensive guide on how to I use the Daily Notes in Obsidian. Comes with a free sample vault to try it out for yourself!


## Things Needed
---
If you want to recreate the daily note that I use, you need to have the following plugins installed:
- Dataview
- Tasks

## What is the Daily Notes Plugin?
---
Daily Notes is a core plugin in Obsidian that creates a note based on the current date. By default, the plugin creates a date in this format: ``YYYY-MM-DD`` although you can change this in the settings.

To create a daily note, click on the **calendar icon** on the left panel or press **Ctrl+P** to open the Command Palette and create the note from there.

For more information on Daily Notes, check out the official Obsidian Help vault in the link below:


## Folder Structure of My Daily Notes
---
I use a folder structure to keep all my daily notes in place. All notes relating to it are inside a main folder called Diary.


Here is an explanation for each folder and note as seen in the screenshot:
- 📂 **_templates:**
	- This is the folder that houses the Daily Note template. I've put an underscore so that this folder appears on top of the navigation panel.
- 📂 **Diary:**
	- This is the main folder containing all the daily notes, index, and log notes.
- 📂 **Daily Notes**
	- This contains all my daily notes.
- 📂 **Yearly Notes**
	- This contains all my yearly notes that I use to create annual reviews and answer the 40 Questions to Answer Every Year.
- 🗒️ **00 Daily Notes Hub**
	- This is the main index or hub note that I use. Think of it as the homepage for your daily notes.
- 🗒️ **00 Media Log**
	- This is a subpage for the hub note that tracks all the media I read and/or watch listed from a daily note. Think of the log notes as pages in a website (like an about page or contact us page.)
- 🗒️ **00 New Discoveries Log**
	- A subpage that tracks all the new discoveries I found from the daily notes.
- 🗒️ **00 Ship's Log**
	- A subpage that tracks all life events and progress from my personal projects.
- 🗒️ **00 Tasks Log**
	- A subpage that tracks all tasks listed in the daily notes.
- 🗒️ **00 Workout Log**
	- A subpage that tracks all workouts performed.

> 💡 The zeroes ("00") are just my way to sort the index and log notes so they appear to the top when browsing my vault in file explorer.

## How I Use the Daily Notes
---
My Daily Note consists of two H2 headers: New Discoveries and Ship's Log.

### New Discoveries
The New Discoveries header is where I add interesting and noteworthy stuff that I find in the Internet (or somewhere else). 

Each new discovery has an emoji that I use as a signifier. Here is an explanation for each signifier:
- 💡 = A general new discovery
- 📕 = Fiction book
- 📘 = Nonfiction book
- 🗿 = Anything related to Obsidian (tips, apps to use in conjuction, codes)
- 🛠 = Tool or resource (useful websites, apps, or software)
- 🎶 = New music
- 🏋️ = Anything related to fitness
- 🎨 = Anything related to art

Every new discovery has the ``NewDiscovery::`` inline field included. This lets me track each entry on the ``00 New Discoveries Log``.



### Ship's Log
The Ship's Log header is where I note down everything I did on a day. These activities are divided into six H3 headers:
- **Tasks Log**
- **Happenings**
- **Personal Projects Log**
- **ReadingLog**
- **VideoLog**
- **Workout Log**

#### Tasks Log
**Tasks Log** is my to-do list. Each entry is written this way:
``- [ ] ❗RemindMe/Life Appointment with so-and-so``
I use nested tags to categorize each task whether it's a task related to this vault or a task to do in real life. If a task is related to a personal project like a blog or video for example, you can use ``RemindMe/BlogName`` or ``RemindMe/VideoChannelName``.

#### Happenings
**Happenings** is where I note down any accomplishments or noteworthy events that happened. You can also use signifiers here like in the New Discovery header to denote a specific event. Each entry has the ``LifeEvent::`` inline field.
``- LifeEvent:: Dentist appointment today. ``

If you are journaling, use ``<br>``  at the end of each paragraph so that they don't break when displayed in the ``00 Ships Log`` log note. Here is an example:
``- LifeEvent:: I went to the bookstore today and saw a lot of new titles. I bought How to Take Smart Notes and a bunch of manga. <br> I saw a cat on the way home. It is very cute. ``

When displayed in the ``00 Ships Log`` log note, Dataview will add a line break in between the two paragraphs. 


#### Personal Projects Log
The **Personal Projects Log** is where I note the progress and ideas for my personal project (this blog!). Each entry has the ``PersonalProjects::`` inline field.

``- PersonalProjects:: ✍️ How I Use the Daily Notes Plugin - Moved to WIP today!``

Much like in the New Discoveries, I use signifiers to denote the status of each project:
- 💡 = Ideas
- ✍ = Work-in-progress projects
- 🛠️ = Polishing (Example: Run everything on Grammarly for articles or add post-processing effects for videos)
- 📸 = Adding screenshots in articles
- ✅ = Published articles
- ❗ = Articles that need to be updated



#### Reading Log
The **Reading Log** is where I note down the articles and books I read. Each entry has the ``ReadingLog::`` inline field.

Here is an example of what my Reading Log would usually look like:
```
- ReadingLog:: ✅ Dragon Ball Z - Finished all volumes!
- ReadingLog:: 📖 One Piece - Chapter 160
- ReadingLog:: ✍️ You Are What You Consume - Interesting article. I should make a literature note out of this.
```

Here is an explanation for each signifier:
- ✅ = Finished book
- 📖 = A "currently reading" book. For manga or comics, you can add the last chapter, volume, or issue that you read.
- ✍️ = For web articles that I've read but still need a literature note.

For audiobooks, I still add them under the Reading Log but use the ``ListeningLog::`` inline  field.

#### Video Log
The **Video Log** works the same way as the Reading Log. Instead of an open book (📖) emoji as a signifier for currently reading books, I use the TV (📺) emoji for currently watching videos. I use the ``VideoLog::`` inline  filed for this section.

```
- VideoLog:: ✅ Did you see that? - Cute cat video
- VideoLog:: ✍️ How to Learn - Need to make literature notes
- VideoLog:: 📺 The Century of the Self - 0:1:34 timestamp
```


#### Workout Log
The **Workout Log** is where I note down the workouts I did for the day. I use the ``WorkoutLog::`` inline field and structure each workout like this:

```
- WorkoutLog:: <br> Deadlift = 4 x 7 (Weight) <br> Lat Pulldown = 3 x10 (Weight) <br> Overhead Press = 3 x 10 (Weight)
```

### Putting it All Together
At the end of each day, I add a ``Title:`` YAML frontmatter and a ``Summary::`` inline field describing what happened and other notable things. To add ``Title:`` YAML frontmatter, type the following on **top of the daily note**.
```
---
Title:
---
```

These two YAML fields will be displayed in the ``00 Daily Notes Hub``.



## How I Use the Log Notes
The Log Notes are the notes that will display all the inline fields from your daily note. All Log Notes use the Dataview plugin to display the content, except for the Tasks Log which uses the Tasks plugin.

> ❗ If the notes are not showing up in the log note, restart Obsidian.

### Media Log
The **Media Log** is the note that will display all the notes containing the ``ReadingLog``, ``ListeningLog``, and ``VideoLog`` inline fields.

To display them, add the following to the Media Log note:

#### ListeningLog Dataview Code

```
dataview
table ListeningLog as "Log"
from "Diary/Daily Notes/"
where contains(ListeningLog, "")
```

#### ReadingLog Dataview Code
```
dataview
table ReadingLog as "Log"
from "Diary/Daily Notes/"
where contains(ReadingLog, "")
```

#### VideoLog Dataview Code
```
dataview
table VideoLog as "Log"
from "Diary/Daily Notes/"
where contains(VideoLog, "")
```

Here is a line-by-line explanation:
- ``table ListeningLog as "Log"``
	- This tells the Dataview plugin to create a table displaying the ListeningLog YAML field as "Log" on the table.
- ``from "Diary/Daily Notes/"``
	- This tells the Dataview plugin to specifically display from the Daily Notes folder.
- ``where contains(ListeningLog, "")``
	- This tells the Dataview plugin to only display the notes that have the ``ListeningLog`` YAML field. You can change this field to ``ReadingLog`` and ``VideoLog`` to display those.



### New Discoveries Log
This log will display all the ``NewDiscovery::`` inline field from the daily notes.
The Dataview code to display this is similar to the Media Log but replace ``ListeningLog`` with  ``NewDiscovery`` .

Here is the Dataview code to display the inline field.
```
dataview
table NewDiscovery as "Log"
from "Diary/Daily Notes/"
where contains(NewDiscovery, "")
```


### Ship's Log
The **Ship's Log** is used to display all ``LifeEvent::`` and ``PersonalProjects::`` inline fields. The Dataview code used is similar to the above log notes. You only need to change the YAML field in the ``where`` code.

#### LifeEvent Dataview Code
```
dataview
table LifeEvent as "Log"
from "Diary/Daily Notes/"
where contains(LifeEvent, "")
```

#### PersonalProjects Dataview Code
```
dataview
table PersonalProjects as "Log"
from "Diary/Daily Notes/"
where contains(PersonalProjects, "")
```

### Workout Log
The **Workout Log** is where I keep a record of all the workout I did on a specific day. It will display all daily notes that have the ``WorkoutLog::`` inline field.

Here is the Dataview code used to display it:
```
dataview
table WorkoutLog as "Log"
from "Diary/Daily Notes/"
where contains(WorkoutLog, "")
```

### Tasks Log
This is the note that collects all pending tasks from your Daily Notes. Here is the Tasks code to display them:

```
tasks
not done
description includes /Work
path includes Diary/Daily Notes
```

Here is a line-by-line explanation:
- ``not done``
	- This tells the Tasks plugin to display tasks that are not completed.
- ``description includes /Work``
	- If you use nested tags such as ``RemindMe/Work`` for example, the Tasks plugin will only display tasks that have that tag. Remove this line of code if you don't use nested tags.
- ``path includes Diary/Daily Notes``
	- This tells the Tasks plugin to specifically display tasks from the Daily Notes folder.


## How I Use the Daily Notes Hub
---
The Daily Notes Hub note is the index note that links all the log notes. In addition, it also includes the title and summary of notes from this week as well as the list of all daily notes.

### Display this Week's Daily Notes
To display the notes of this week, add the following Dataview code:

```
dataview
TABLE WITHOUT ID link(file.link, " ") + "<strong>" + Title + "</strong><br>" + Summary  + "<br>" + file.link AS Entries
from "Diary/Daily Notes/"
SORT file.name desc
LIMIT 7
```

Here is a line-by-line explanation:
- ``TABLE WITHOUT ID link(file.link, " ")``
	- This tells Dataview plugin to create a table without the link to the note. By default, the plugin creates the note on the left column while the right column is used for the YAML fields.
- ``+ "<strong>" + Title + "</strong><br>"``
	- This tells Dataview plugin to display the Daily Note's ``Title`` in bold. The ``<br>`` adds a line break for the next YAML field.
- ``+ Summary  + "<br>" +``
	- This display the Daily Note's ``Summary`` below the ``Title``. Another ``<br>`` adds a line break for the next field.
- `` + file.link AS Entries``
	- This displays the name of the Daily Note and its link below the ``Summary``. It will also name the Dataview table as "Entries"
- `from "Diary/Daily Notes/"`
	- This tells the Dataview plugin to specifically display the notes from the Daily Notes folder. If you put your daily notes on a folder with a different name, change this text inside the double quotes to match the folder name ("").
- ``SORT file.name desc``
	- This tells the Dataview plugin to sort the files in descending order.
- ``LIMIT 7``
	- This tells the Dataview plugin to limit the number of displayed contents to seven.
> 💡 The plus(+) sign at the end of each code acts as a space in between.

### Display All Daily Notes

If you want to display all your daily notes in descending order, remove the ``LIMIT 7`` from the Dataview code:


```
dataview
TABLE WITHOUT ID link(file.link, " ") + "<strong>" + Title + "</strong><br>" + Summary  + "<br>" + file.link AS Entries
FROM "Diary/Daily Notes/"
SORT file.name desc
```


### Display Daily Notes within a Certain Date
If you want to display your daily notes within a certain range, such as all notes from 2021,  add ```WHERE file.day >= date(2021-01-01) AND file.day <=date(2021-12-31)``` on the Dataview code:

```
dataview
TABLE WITHOUT ID link(file.link, " ") + "<strong>" + Title + "</strong><br>" + Summary  + "<br>" + file.link AS Entries
FROM "Diary/Daily Notes/"
WHERE file.day >= date(2021-01-01) AND file.day <=date(2021-12-31)
SORT file.name desc
```


This code will tell the Dataview plugin to only display notes from January 01, 2021 to December 31, 2021.

## Add Optional Features
---
### Dynamic Previous/Next Daily Note Navigator
If you want to add a navigator on your daily notes, you can add the following DataviewJS code:

```
dataviewjs
/*
    previous/next note by date for Daily Notes
    Also works for other files having a `date:` YAML entry.
    MCH 2021-06-14
*/
var none = '(none)';
var p = dv.pages('"' + dv.current().file.folder + '"').where(p => p.file.day).map(p => [p.file.name, p.file.day.toISODate()]).sort(p => p[1]);
var t = dv.current().file.day ? dv.current().file.day.toISODate() : luxon.DateTime.now().toISODate();
// Obsidian uses moment.js; Luxon’s format strings differ!
var format = app['internalPlugins']['plugins']['daily-notes']['instance']['options']['format'] || 'YYYY-MM-DD';
var current = '(' + moment(t).format(format) + ')';
var nav = [];
var today = p.find(p => p[1] == t);
var next = p.find(p => p[1] > t);
var prev = undefined;
p.forEach(function (p, i) {
    if (p[1] < t) {
        prev = p;
    }
});
nav.push(prev ? '[[' + prev[0] + ']]' : none);
//nav.push(today ? today[0] : none);
nav.push(today ? today[0] : current);
nav.push(next ? '[[' + next[0] + ']]' : none);

//dv.list(nav);
//dv.paragraph(nav.join(" · "));
dv.paragraph(nav[0] + ' ← ' + nav[1] + ' → ' + nav[2]);
```

### Read Later and Watch Later Tracker
You can use the Tasks plugin to create a Read Later and Watch Later tracker on the ``Tasks Log``.

The ``WatchLater`` and ``ReadLater`` entries are written this way:
``- [ ] WatchLater Obsidian Flight School: The Walkthrough``
``- [ ] ReadLater Habits vs. Goals ``

On the ``Tasks Log`` note, add the following code:
```
tasks
not done
description includes WatchLater
path includes Diary/Daily Notes
```

The ``description includes WatchLater`` code tells the Task plugin to specifically display tasks that have the WatchLater tag. Replace the WatchLater tag with the ReadLater tag to display those instead.


## Download the Sample Vault
---
I've created a sample vault that you can play around with and test this workflow for yourself! You can find it in this [Github link](https://github.com/GentryGibson/DailyNotes).


## Credits
---
- blacksmithgu: [Dataview Plugin](https://github.com/blacksmithgu/obsidian-dataview)
- schemar: [Tasks Plugin](https://github.com/schemar/obsidian-tasks)
- SlRvb: [Code for the title and summary for the Daily Notes Hub.](https://forum.obsidian.md/t/slrvbs-journaling-setup/22346)
- mnvwvnm: [Code for adding inline values in Dataview and in a note.](https://forum.obsidian.md/t/reverse-block-reference-possible/22445/4)
- Eleanor Konik: [Basis of the Reading Log in the Daily Notes template.](https://forum.obsidian.md/t/a-template-for-daily-notes/15619)
- Moonbase59: [DataviewJS code for the Daily Notes previous/next navigation links](https://forum.obsidian.md/t/dataviewjs-snippet-showcase/17847/21?u=gibson.)