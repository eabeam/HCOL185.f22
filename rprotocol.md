# Research Protocol 

*[Back to index](index.html)*

*You're about to do a big thing! :muscle: The aim of this assignment is to anticipate and work out as many details as possible to streamline your experience. With these issues out of way, my hope is that the challenges that emerge will be only the most interesting and satisfying to tackle!*

**Due 28 October @ 1:10pm **

**Protocol Template: [HCOL185_research-protocol-template.docx](HCOL185_research-protocol-template.docx)**



[TOC]



## Instructions 

Download the [attached template](HCOL185_research-protocol-template.docx) to generate detailed protocol of all the *implementation* steps of your study, building off your research methdology. Make sure to address or incorporate suggestions/comments in response to your submitted research methodology. 

Submit the following: 

1. Completed [research protocol template](HCOL185_research-protocol-template.docx)
2. [Data collection template](#data-collection-template): submit as separate attachment
3. Template and sample of all submission materials: the template includes a list of potential materials 

Some elements will require a bit of experimentation to figure out how best to proceed. I've included some advice and instructions on possible directions below. 

For a bigger-picture discussion of considerations, I recommend this (relatively brief) chapter by Joanna Lahey and Ryan Beasley, ["Technical Aspects of Correspondence Studies"](https://www.nber.org/system/files/working_papers/w22818/w22818.pdf)



## Data collection template

Make sure that each submission has a numeric id. This could be as simple as S1–S800, or it could be more complex, like LA001–LA099 for Los Angeles submissions and NY001–NY099 for NY submissions. 

- Make an excel file with **one row per submission**. 
- List the ID :point_up: , the resume characteristics and/or number, and any relevant employer/recipient characteristics (name of employer, type of employer, etc.) 
- Record the date and time submitted. 
  - You can do this with keystrokes! 
    - On a Mac or PC  ==`control + ;`== will [display the date](https://excel-hack.com/today-date-shortcut/).  
    - Then, to [display the time](https://excel-hack.com/today-date-shortcut/), you can type ==`command + ;`== on a Mac or ==`ctrl + shift + ;`== on a PC
- Make a column for whether you received a call-back (1/0). 
  - You may also want other columns for callbacks: date of callback, time of callback, nature of callback (if multiple options, like phone/email/text)
  - You may want a column for the text of the response (if you plan on doing some sort of textual analysis). If so, literally copy and paste the text into it.

## Additional Guidance



### From randomization to data

For most projects, you will start with a template that has some randomizable elements. You will need to do the following: 

1. Identify possible values to fill in randomized element (Greg, Emily, Steve, Jamal, etc.)
2. Randomize those elements
3. Insert those elements into templates to generate unique resumes/letters/responses 
4. Submit these responses 
5. Wait ... 
6. Record data!

Steps 2–3 can get very complicated very quickly. 

If you are comfortable with learning new techy things, Lahey and Beasley have made a ["resume randomizer"](https://github.com/beaslera/resumerandomizer) that robustly does step 2 and 3. 

1. There is a `.exe` program version (runs on Windows only). You can download a zip file with all necessary materials  [here](https://www.dropbox.com/s/wj2bhl5mhqn5xsh/resume-randomizer_version_20.zip?dl=0) (no longer available on NBER archive). It is very important you follow the detailed instructions, included [here](https://www.dropbox.com/s/type9swwg65hye0/Steps%20to%20using%20Resume%20Randomizer%20Program.docx?dl=0).[^fn1] *This worked in 2016, but I'm not 100% sure it is compatible with new OS versions*
2. The source (python) code is available at Beasley's [repository](https://github.com/beaslera/resumerandomizer). This is extremely versitile, but you would want some python familiarity to figure out what you need to do.

[^fn1]: We used  this program in a [correspondence study back in 2015/6](https://drive.google.com/file/d/14R9qXCckYSzQPhNg1H2MEppl3faxNDRc/view), but because my co-author generously took care of this project step , I'm not that familiar! 

If these approaches are not for you, continue on!



### Assembling materials 

Note that so long as you can identify what person/subject is responding to which submission, you only need a few phone numbers and e-mails. (With a matched-pairs design, you need more, but not *that* many more). Reuse them and save yourself a lot of hassle!

#### What if i need phone numbers for e-mail verification? 

Try out [quackr.io](https://quackr.io/temporary-numbers) :duck: Note that this isn't suitable as a phone number for people to respond to!

#### What if I need phone numbers to receive responses? 

I strongly recommend *not* using your personal phone numbers.

- [Google voice](https://voice.google.com/u/0/signup) will give you a free number that forwards to your phone. This obscures your own phone number, and allows you to select an area code of your choice. However, you cannot do multiple numbers

- [Textfree](https://textfree.us/) will work give you a free phone number via [iOS](https://apps.apple.com/us/app/text-free-texting-app-sms/id399355755) or [Android](https://play.google.com/store/apps/details?id=com.pinger.textfree) app. Similar services include [TalkU](http://www.talkyou.me/en/index.html), and Talkatone.[^fn2]

- Remember that you don't need to have a lot of these - it's fine to reuse numbers ALOT (so long as you have a way to identify which submission received a callback )

  [^fn2]: I have never used these.



### Randomization

At some point, you will need to randomize something. There are many ways to do this. My recommendation for a *simple* and robust way to do this is in Excel. It has disadvantages - not replicable - but it gets the job done. 

The World	 Bank's DIME unit has a [detailed review](https://dimewiki.worldbank.org/Randomization_in_Excel), and I've included a short **demo** below

> Here are the steps of doing successful **randomization using Excel**:
>
> 1. **Randomization Rule.** For example = the lowest 50% will be treatment, the rest will be assigned to control, etc.
> 2. **=rand().** Assign random numbers to each observation. While doing this, use "paste values" to stop recalculating the randomization.  ==**:rotating_light: this means you have to generate the `rand()` values, and then highlight them, select "copy" and then "paste special" in order to paste the values. Else they will keep changing! :rotating_light:**==
> 3. **Sorting.** Sort the random numbers from the lowest to the highest.
> 4. **Order.** Created an ordered serial number. If you need to balance the data, then first sort by the strata, then by the random values.
> 5. **Assignment.** Assign groups using either the ` `mod` ` or the  ` if ` formulas.
> 6. **Finish.** Save the record.



#### **DEMO: Randomization in Excel**

<iframe width="560" height="315" src="https://www.youtube.com/embed/KE2KViKAeSI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>



#### Randomizing multiple elements 

If you have one or two stock templates, and then you are randomizing one element, then :point_up: will serve you well. However, if you have multiple elements, this can get very confusing very quickly. 

My recommendation is a two step process. 

Generate a series of numbered resume templates. The number of templates equals the number of potential combinations across *all* randomized units. 

For example, if you are randomizing name (4 names, 2 white & 2 black) but also university (2 choices) and primary employer (3 choices), then you have $4*2*3 = 24$ possible templates. Number them R1 – R24. Then, randomly assign each posting (or submission) to one of those templates using the above process in Excel. 

### Data security 

I've included a write-up of how to approach data security [here](data-security.html)

## Grading

Each item listed below is worth 5 points. For each item, you will earn 4 points if the necessary elements are included and complete. You will earn 5 if they are thorough, are *ex-ante* likely to succeed, and reflect critical thinking about potential problems and challenges. 

**Key items:** 

|      | Key items (50 points total)             | Description                                                  |
| ---- | --------------------------------------- | ------------------------------------------------------------ |
| 1    | Key outcomes and hypothesis tests       | See protocol template                                        |
| 2    | Participant selection criteria          | ---                                                          |
| 3    | Randomization                           | ---                                                          |
| 4    | Building applicant profiles             | ---                                                          |
| 5    | Submission and data collection profiles | ---                                                          |
| 6    | Planned analysis                        | ---                                                          |
| 7,8  | Submission materials                    | x2 points: Include both templates and samples                |
| 9    | Data collection template                | Separate Excel file1                                         |
| 10   | Timeline and data management plan       | See protocol template and [data management](data-management.html) |
|      |                                         |                                                              |









***[Back to index](index.html)***