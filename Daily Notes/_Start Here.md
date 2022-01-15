# Start Here

> Thank you for downloading the sample vault! This note serves as a cheat sheet to use this Daily Notes setup. See the [Comprehensive Guide](https://thebuccaneersbounty.wordpress.com/2022/01/05/how-i-use-the-daily-notes-plugin-a-comprehensive-guide/) for more information.  <br>
> Created by 🏴‍☠️ [Gentry Gibson](https://thebuccaneersbounty.wordpress.com/about/) |  📝  [Other Tutorials](https://thebuccaneersbounty.wordpress.com/tutorials/)


## Daily Note Inline Fields
---

> 💡 Remember to remove the **`backticks(```)`** in the inline fields below if you want to activate them!

The following inline fields are the ones you input in your daily note->([[2022-01-04]]) for them to appear in the corresponding log notes.

- ``NewDiscovery::`` 
	- Enter this inline field to add an entry in the [[00 New Discoveries Log]]
- ``[ ] #❗RemindMe Task description``
	- Enter this task to add it to the Task List section of the [[00 Tasks Log#Tasks List]]
- ``[ ] #ReadLater Book or web article to read later ``
	- Enter this task to add it to the Read Later section of the [[00 Tasks Log#Read Later]]
- ``[ ] #WatchLater Video or movie to watch later``
	- Enter this task to add it to the Watch Later section of the [[00 Tasks Log#Watch Later]]
- ``LifeEvent::`` 
	- Enter this inline field to add an entry in the Life Happenings section of the [[00 Ship's Log#Life Happenings]]
- ``PersonalProjects::``
	- Enter this inline field to add an entry in the Personal Projects section of the [[00 Ship's Log#Personal Projects]]
- ``ListeningLog::``
	- Enter this inline field to add an entry in the Listening Log (for audiobooks) section of the [[00 Media Log#Listening Log]]
- ``ReadingLog::``
	- Enter this inline field to add an entry in the Reading Log (for books and web articles) section of the [[00 Media Log#Reading Log]]
- ``VideoLog::``
	- Enter this inline field to add an entry in the Video Log (for videos and movies) section of the [[00 Media Log#Video Log]]
- ``WorkoutLog::``
	- Enter this inline field to add an entry in the [[00 Workout Log]]
- ``Summary::``
	- Add a summary for it to appear in the [[00 Daily Notes Hub]]
- ``Title:`` 
	- Add a title of the daily note for it to appear in the [[00 Daily Notes Hub]]. You need to switch to **Editing Mode** (Ctrl-E or Command-E) and **scroll up to the top of the note** to find this metadata.

## Log Notes Dataview Codes
---
> 💡 Remove the space between the three **`backticks (```)`** and the `dataview` or `tasks` word if you want to activate the codes below!

### [[00 Daily Notes Hub]]
#### Display This Week's Notes
```
dataview
TABLE WITHOUT ID link(file.link, " ") + "<strong>" + Title + "</strong><br>" + Summary  + "<br>" + file.link AS Entries
from "Diary/Daily Notes"
SORT file.name desc
LIMIT 7
```

#### Display Notes from 2022
```
dataview
TABLE WITHOUT ID link(file.link, " ") + "<strong>" + Title + "</strong><br>" + Summary  + "<br>" + file.link AS Entries
from "Diary/Daily Notes"
WHERE file.day >= date(2022-01-01) AND file.day <=date(2022-12-31)
SORT file.name desc
```

### Display Notes from 2021
```
dataview
TABLE WITHOUT ID link(file.link, " ") + "<strong>" + Title + "</strong><br>" + Summary  + "<br>" + file.link AS Entries
from "Diary/Daily Notes"
WHERE file.day >= date(2021-01-01) AND file.day <=date(2021-12-31)
SORT file.name desc
```

### [[00 Media Log]]

#### Display Listening Log Entries
```
dataview
table ListeningLog as "Log"
from "Diary/Daily Notes"
where contains(ListeningLog, "")
```

#### Display Reading Log Entries
```
dataview
table ReadingLog as "Log"
from "Diary/Daily Notes"
where contains(ReadingLog, "")
```

#### Display Video Log Entries
```
dataview
table VideoLog as "Log"
from "Diary/Daily Notes"
where contains(VideoLog, "")
```

### [[00 New Discoveries Log]]

#### Display All New Discoveries
```
dataview
table NewDiscovery as "Log"
from "Diary/Daily Notes"
where contains(NewDiscovery, "")
```

### [[00 Ship's Log]]

#### Display All Life Events Entries
```
dataview
table LifeEvent as "Log"
from "Diary/Daily Notes"
where contains(LifeEvent, "")
```

#### Display All Personal Projects Entries
```
dataview
table PersonalProjects as "Log"
from "Diary/Daily Notes"
where contains(PersonalProjects, "")
```

### [[00 Tasks Log]]
#### Display All #RemindMe Tasks Entries
```
tasks
not done
description includes RemindMe
path includes Diary/Daily Notes
```

#### Display All #ReadLater Tasks Entries
```
tasks
not done
description includes ReadLater
path includes Diary/Daily Notes
```

#### Display All #WatchLater Tasks Entries
```
tasks
not done
description includes WatchLater
path includes Diary/Daily Notes
```

### [[00 Workout Log]]
#### Display All Workouts
```
dataview
table WorkoutLog as "Log"
from "Diary/Daily Notes"
where contains(WorkoutLog, "")
```