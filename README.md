java c
Vampire   Hunting
COMP0015   2024-2025 Term   1 Coursework – 60% of the   moduleThis   document   explains   the   arrangements   for   the   coursework.   You   will   create   an   application   that analyses a dataset   to   determine   how   a   vampire   infiltration   spreads   based   on   testing   and   contact   tracing   data.   This   document   is   fairly   lengthy;   do   not   be   deterred   by   this.   The   coursework   has   been   carefully   designed so that you can   complete   it   part   by   part and   know that you   have the correct functionality   at   each   point.   Each   part   is   described   in   its   own   section.
Strong suggestion: start your coursework as   early   as   possible   to   give   yourself time   to   resolve   issues   you   encounter.
Deadline
December   13,   2024 at   16:00   (4pm –   UK time).
How to submit your   workSubmit   your    contact.py   file   at   the   assignment   link   on   Moodle.   Do   not   submit   any   other   files.   Do   not   upload   a   folder   containing   your   files   because   this   can   cause   compatibility   issues   for   the   marking   team.   You   must   ensure   that   your   program works   properly on your own computer   before   you   submit   the   code.
Important:   make sure your student   number   (not your   name)   is   included   in the comments   at   the   top   of   your   program.
Testing
You   are   responsible for   testing   your program carefully.   Make sure that you   have thought about all the   things   that   can   go wrong and test your   program to ensure   that   you   know   it   works   correctly   in   all   circumstances.
However,   as   an   aid,   we   have   developed   a   web-based   testing   service.       We   strongly encourage you   to   take advantage   of this service.    More details can   be found   in   Appendix   1,   the   following   points   are   key:
1.          The tool   may   be extremely   helpful—in   previous terms, students   in aggregate   used the   service   5,000+   times.
2.          Nevertheless, the tool does   not   provide   any guarantee   of   a   final   grade.
a.          Your final submission will   be tested on   additional   datasets,   which   can   change   scores.
b.         Your final grade will   include   marks for comments/style, which   can   change   scores.
c.          We   reserve   the   right   to   modify your grade after   manual   inspection.      For   example,   attempts   to “trick”   the autograder will   result   in zero   marks.
d.          If    your   code   does    not   work   with   the   autograder,   we   may   attempt   to   modify   it   to   award   a   non-zero   grade.   If   successful,   we will deduct some   marks   (typically   10-20%, although we   make   no   guarantees).   Accordingly,   please   make sure your code works   properly with the   autograder   before   submitting.
3.          We do   not guarantee that the testing   service will   always   be   available   (e.g.,   the   server   may   crash).
4.          The testing service tests each part individually. If you get stuck on one section but can    get   something   working   for   a   later   section,   then   you   may still   be able to get   marks for that   later   section,   even   if   running   it   on   your own   machine   (which will   use the   pre-defined main   ()   function from the template)   doesn’t work.
5.         The   testing   service   can   sometimes   get   confused   by   non-ASCII   characters.      Accordingly,   and   with   apologies,   avoid   using Amharic/Arabic/Chinese/Thai/etc. characters   in your code, even within   comments.
Assessment
You   are   expected   to   show   that   you   can   code   competently   using   the   programming   concepts   covered   in   the   course   including   (but   not   limited to): the   use of files, strings,   lists, dictionaries,   sets,   conditions,   loops,   and   functions.   Marking criteria will   include:
●         Correctness – your code   must   perform. as specified.
●         You   must apply   Python concepts appropriately.
●          Programming style. – see section ‘Appendix   2   Style   Guide’ for   more   detail.
●         Your assignment will be marked using the rubric in Appendix 3. This is the standard rubric used in the   Department of    Computer    Science.    Marks for your project work will be awarded for the   capabilities    (i.e.   functional   requirements)   your   system   achieves,   and   the   quality   of   the   code. Categories 5 and   6 of the   rubric   will   be   used for coding assignments.
Before starting your   assignmentYou   are   provided   with   some   starter   code   in   the   file   template.py.   Your   first   action   should   be   to   make   a   copy   of   this   code   into   a   new   file,    contact.py,   where   you   will   work   afterwards.   You   have   also   been   given   a   helper   file   format_list.py;   you   shouldn’t   modify   this   but   will   need   to   have   it   in   the   same   directory.      You   have   also   been   given   some   text   input   files   containing   infiltration   data   (Data   Set0.txt   …   Data   Set5.txt)   and   associated   text   output files   (Data   Set0-out.txt   … Data   Set5-out.txt).    You should   put these   in the same   directory   also.Before   you   start   writing   code,   read   through   this   entire   document   so   that   you   have   a   sense   of   what’s   coming   and   can   start   to   think   about   how   different   parts   are   going   to   work   together.       The    overall   task   is   more   complex   than   anything   you’ve   done   so   far,   but   it’s   also   been   broken   into—forgive   me—bite-sized   pieces.       In   section   22,   there   is   a   summary   of   all   of   the   different   functions   you   have   to   write,   the   number   of   lines   in   the   official   solution   (just   to   give   yourself   a   sense   of   relatively difficulty   —your own solution   might   be quite   a   bit   longer,   and   that’s   ok),   and   an   informal   sense of which   parts are a   bit trickier than   others   (sometimes   short   functions   can   be   trickier   than   long   ones).
Keep   in   mind   that   the   testing   service   you   have   access   to   (see   appendix   1) and the way   we will   do the   grading   will   be   function-by-function.    So, even   if you can’t get   some   critical function   working   correctly,   work   on   other   functions.
Goodluck   and   enjoy!
Running the contact tracing   programThere   are   two   ways   to   run   the   program   from   the   terminal   depending   on   whether   you   want   to   provide   the   data file   name   on   the   command   line   or   whether   you   want   the   user   to   be   prompted   for   the   file   name.   The   code   in   main()   contains code to   handle this.    Important: you   should   not   edit   the   code   in   main().
Entering a file   name on the   command   line   (suggested)
On Windows,   run the   program   in the terminal, specifying the data   file   name:
   
or on   macOS   type:
   
The   meaning of the terms on   this   line   is:
python or   python3
The   python   interpreter.   On   macos   this   will   be   python3   and on Windows, this will   be   py   or   python.
contact.py
The   name of the   python   program.
DataSet0.txt
Name of the   data   file.
Table 1    Running   the program, specifying   the   file name on   the   command line
Prompting the   user for a file   name   (possible,   but   perhaps a   bit   painful to   test)
To   prompt the   user for a file   name, simply   run the   program   in your   editor   (IDE)   as   you   would   normally.
Section   1   : OrientationYou   have   been   given   several   files containing testing and contact tracing   data for   vampire   infiltrations.      This   data   has   a   “preamble”    (initial    part),   followed    by   a    list   of   testing   and   contact   tracing   data   for   a   series   of   days    (“body”).       The   format will   be explained   in detail   below.In   order to work with the contact tracing   data, you   will   need   to   load   a   data   file   storing   contact   tracing   data   and   create   appropriate    data    structures      such      as      a      dictionary      or      a       list.    These      data      structures      can       be       used    to    identify    the   relationship   between the   individuals   in the data.Many    of    the      sections       require    you      to       print    out      data      after    you      have      calculated      it,      often      in    separately-specified   functions.          Sometimes      functions      will       require    you    to    check    for    some      kinds      of      data      errors,      print      specified      error   messages, and then exit   by calling   s   ys.exit   ().
Important:   do   not   modify   the   main   ()   function;   all   of your work should   be   in the other functions   as   specified   in the   various sections.    Do   not add   code that just   runs   at   the “top   level”.   All   of your   code   should   be   inside   functions.Important:    Part    of    our    testing    procedure      is    to      run   functions      individually.             Make    sure    that   your   function    names,   parameters,   and   return   values   don’t   change   from   our   specification.       Moreover,    make    sure    that   your   functions   do   what   they   are   supposed   to   do,   rather   than   e.g.,   trying   to   do   one   big   function   that   does   the job   of   several   of   our   specified functions.
Important:   Ensure that your   program’s output   matches exactly   the output   given   to   you   unless   otherwise   specified.
Important:   do   not   import any additional   packages;   lines 7-9 of the   template.py   file   already   imports   sys,   os.path,   and format_list; that’s all you   need   (and all you are   allowed).
Data filesThe   files   (as   well   as   your   assignment’s   expected   output   for   each   file)   are   posted   on   moodle   with   the   assignment   information.   Each   file   ends   with   the   .txt   extension.   You   can   open   the   files   in   Visual Studio Code or   in a text   editor   to   see the   contents.
PreambleThe   preamble   begins   with   a   (comma-separated)   list   of   individuals   (without   specifying   which   are   humans   and which are vampires).    These are   all   of the   individuals that   may   appear   in   the   rest   of   the   dataset.      On   the   next   line,   the   preamble   gives   the   number   of   days   of   data   that   will   follow.       For   example,   a   valid   preamble   would   be as   follows:Bella,    Edward,    Jacob,    Carlisle,   Alice,   Emmett,   Charlie,   Renee,   Jessica,
Angela
4
N.B.    Sometimes    spaces    are    included   around    names   to   aid   human   readability   as   in   the   above   example;   these   are   optional,   but your code will   have to   remove them   if they   appear.    The   strip   ()   method   can   help   you   do this.Important:   names   may   include   a   mixture   of   upper   and   lowercase   letters,   as   well   as   some   special   characters such as   dashes.       Names   will   not   include   numbers,   commas, colons, the   newline character   (“\n”), tabs   (“\t”), or the   symbol   #.   Spaces   may appear within   a   name, e.g.   “Kuan Yew”,   but   not   at   its   beginning   or   end,   e.g.   no   “ Kuan   Yew   ”.
DayUnlike   in   some   of   the   legends,   our   vampires   are   able   to   move around during the day,   rather than   sleeping   in   coffins.   (Some   of them do sleep   in coffins at   night,   but   that’s   not   important   for   this   exercise.)      We   divide   each   of   our   days   into   two   parts   (AM,   when   testing   occurs;   and   PM,   when   contact   occurs).    Each day   has the following format.      On   the   first   line   is   a   comma-separated   list   of   people   who   have   been   given   a   vampirism   test   in   the   morning   (AM)   of   that   day   (perhaps   a   brief   exposure   to   sunlight);   the   result   of   the   test   (“V”   for   vampire   or   “   H”   for   human)   is   given   after   each   name, separated   by a colon.      If   no one   is   given   a   test   on   a   given   day,   this   line   will   be   the   special   string   ##.
On   the   second   line   is   a   number   of   groups   of   people   who   had   interactions   in   the afternoon   (PM) of that day.      On the   third and following   lines are comma-separated   lists   of   individuals who   have   been   in   contact.      To   keep   things   simple:
1.          Each   individual can   be   in at   most   one   contact   group   on   a   given   day.
2.          On   the   other   hand,   there’s   no   need   for   an   individual   to   meet   with   anyone   on a given day;   in that   case,   their   name   won’t   appear   in   any   contact   list   for   that   day.    When vampires are   in the   neighbourhood, staying   home   alone can   be the   safest   option!
3.          All   people   in a group   meet simultaneously   (perhaps to   play a   game   of   baseball).
Here’s an example   of   a   valid   day:
Edward   : V, Bella   :   H,   Jacob   :   H,   Jessica   :   H   3
Bella, Edward
Charlie,   Jacob
Alice, Renee
N.B. Again, spaces can appear to   aid   human   readability;   in this   case   you’   ll   have   to   remove   them.
To complete the demonstration of the   input,   here   are the   remaining   three   days   promised   in   the   preamble   above:
Bella   : H,   Jacob:H, Alice   :V,   Charlie:   H   2
Bella, Edward,   Charlie
Angela,   Jessica
Emmett   : V,   Renee   :   H,   Jessica   : V
0
Bella   : V,   Charlie:   H   2
Bella, Edward, Charlie,   Jessica, Angela
Jacob,   Renee
Notice   that   on   the   third   day   everyone   stayed   home   (0   contract   groups).       None   of   the   days   had zero tests   (which we   would   have   indicated with   ##).
Note: the above file   is   in fact one of the   input   testing   files   we   give   (Data   Set1.txt).
Section   2: Check the file   exists   (1   mark)
Take a   look at the   following   code   in   main():
   
The   python   code   sys.exit()   will   cause   the   program   to   terminate   if   the   file   cannot   be   opened   and   read.   Important   : do   not change the code   in   main().The   function   file_exists()   takes   the   file   name   given as a   parameter, and checks that   the   file   exists.   Your   first   task   is    to    complete   the   function   file_exists().   The   function   file_exists()must    return   True   if   the   file   exists   and   False   if   it does   not.   Hint:   use the function   isfile()   from the   python   library os.path.
Section   3: Create a structure to   hold the   input   data   (6   marks   for   correctly   代 写COMP0015 2024-2025 Term 1 CourseworkPython
代做程序编程语言storing   the data +   1   mark for correctly   printing the   error   message   when   needed)Complete the function      parse_file(). This function takes a file   name   as   a   parameter,   reads the   file   line   by   line   and   creates a data structure to   represent the   input.    The   structure   has   the   following   format:   at   the “top”   it   is   a pair.      The      first element of the   pair   is a list   of   names   (the   participants)   in   the   order   given   in   the   file.    The   second   element   of   the      pair   is a list of   pairs; each   list   cell will   correspond   to   a   given   day.
Within each   list-pair, the first element should   be   a   dictionary whose   keys   are   the   names   of   those   tested   for   vampirism   and whose values are the   Booleans True   (that   is, a   vampire,   indicated   by “V”   in   the   input   file)   or   False   (that   is,   a   human).    The second element of a   list-pair   is   a   list   of   lists,   with   each “outer”   list-element   being   an “inner”   list   of those   groups who were   in contact on that   day.    After   you   finish   processing   the   file,   make   sure   to   close   it,   and   then   return   the structure you’ve created.    Here’s   the   structure   we’d   expect   for   the   sample   file   given   above,   as   printed   by   Python:
(   [   'Bella   ',   'Edward   ',   'Jacob   ',   'Carlisle   ',   'Alice   ',   'Emmett   ',   'Charlie   ',
'Renee   ',   'Jessica   ',   'Angela   '],   [   ({   'Edward   ': True,   'Bella   ': False,   'Jacob   ':
False,   'Jessica   ':   False},   [   [   'Bella   ',   'Edward   '],   [   'Charlie   ',   'Jacob   '],
[   'Alice   ',   'Renee   ']]),   ({   'Bella   ': False,   'Jacob   ': False,   'Alice   ':   True,
'Charlie   ':   False},   [   [   'Bella   ',   'Edward   ',   'Charlie   '],   [   'Angela   ',   'Jessica   ']]),
({   'Emmett   ': True,   'Renee   ': False,   'Jessica   ':   True},   []),   ({   'Bella   ':   True,
'Charlie   ':   False},   [   [   'Bella   ',   'Edward   ',   'Charlie   ',   'Jessica   ',   'Angela   '],
[   'Jacob   ',
'Renee   ']])])
If the file   isn’t somehow formatted correctly – for   example,   if one   of   the   numbers   isn’t   a   number   when   you   convert   it   to an   integer – then   print the error   message   Error found   in   file,   aborting.      Then, exit   (using   s   ys.exit   ()).
Important   : for this section,   and all   sections   that   follow,   you   should   print   to   the   screen   (rather   than,   e.g.,   writing   your   results to a file).    Also,   it   is critical that   you   produce   the   exact   error   message   we   specify   to   get   the   mark.
Section 4   :   Pretty-print the data structure   (4   marks)
Please fill   in the function   body of the function pretty_print_infiltration_data   (data).      By “   pretty,”   what we   mean   is   in a   more   human-readable format than the   Python default   shown   above.      Specifically,   we’re
expecting something   in the following exact   format   (the   reason   one   line   is   in   red   is   explained   below):
Vampire   Infiltration   Data
4 days   with   the   following   participants:   Alice,   Angela, Bella,   Carlisle,
Charlie, Edward, Emmett, Jacob,   Jessica   and   Renee.
Day 1   has   4 vampire   tests   and   3   contact   groups.
4   tests
Bella   is   human.
Edward   is   a vampire!
Jacob   is human.
Jessica   is   human.
3   groups
Bella   and   Edward
Charlie   and   Jacob
Alice   and   Renee
Day 2 has   4   vampire   tests   and   2   contact   groups.
4   tests
Alice   is   a   vampire!
Bella   is   human.
Charlie   is   human.
Jacob   is human.
2   groups
Bella, Charlie   and   Edward
Angela   and   Jessica
Day 3 has   3   vampire   tests   and   0   contact   groups.
3   tests
Emmett   is   a vampire!
Jessica   is   a   vampire!
Renee   is   human.
0   groups
Day 4   has   2 vampire   tests   and   2   contact   groups.
2   tests
Bella   is   a vampire!
Charlie   is   human.
2   groups
Angela, Bella, Charlie,   Edward   and   Jessica
Jacob   and   Renee
End   of   Days
There are a   lot of   parts   here,   so   let’s take   them   one   at   a   time.
As you can see, the   printout   begins with “Vampire Infiltration   Data”   and   ends   with   “End   of   Days”.            The   next   line,   in   red,   is actually a single   line,   but to   avoid   small fonts   in   this   writeup,   it   appears   to   be   broken   over   two   lines.    (You shouldn’t try   to change   the   printing   colour   in   your   solution;   it’s just   here   for   clarity   on   this   issue.)      All   of
the other   lines for this dataset are   short   and   thus   do   not   have   this   issue.
There are   many   lists of   participants, separated   by commas   and   with   a   final “and”.      You   have   been   provided   with
module   format_list.py   which contains the function   format_list   (data).   Use the function   format_list   (data)   to format a   list as a   string   in this   way.
The second   line   (in   red)   in the   printout gives the   information that was   in the   preamble   of the   input   file.      Afterwards,      we   have a series of days,   which   begin   with the   day   number,   the   number   of   vampire   tests,   and   the   number   of   contact   groups.    Notice that when there   is   only   1 test   or   group,   there   is   no “s”   after “test”   or “group.”      In   general,   we   make               sure to get all of the   plurals correct,   in   the   printout.      Hint:   you   should   too.
Within a day, we start   by   repeating the   number   of   tests.      The   line   is   indented   to   the   right   by   two   spaces.      Then   we               give the   results of each test, with the   participants   grouped   in   alphabetical   order.      Participant   results   are   indented   by   four spaces.    Then we   repeat the   number of groups   (two   space   indent),   and then   a   list   of   each   of   the   groups   (four
space   indent).
Hints: There are a   number of other   things   to   be   careful   of,   like   periods   at   the   end   of   sentences   (but   not   at   the   end   of   lists), and so forth.      It’   ll take some   careful   work   to   make   sure   you   have   the   format   exactly   right.Other   than   within   a   list   of   test   results,   participants   should appear   in the same order as   the   test   file.      (The   test   results   were   stored   in   a   dictionary,   which   does   not   guarantee   that   order   will   be   preserved.       Rather   than   require   that   you   somehow   restore   the original order, we simply   require that   you   alphabetize   the   participants.      Reminder:   if you   have   a   list mylst, then mylst.sort   ()   will sort   it; there are other   ways   to   sort   it   too.)Important:   check   the   format   of the output expected for the files given   to   you;   unless   we   specify   otherwise   we   expect   you   to   follow   this   format   exactly.   The   output expected for each data file   can   be   found   in   the   corresponding   file   name   with the word “out”   in the   name.   For example: the output   for   DataSet1.txt   is   given   in   DataSet1-out.txt.
Section   5   : Write   lookup   helper function   (1   mark for correctness)
To analyse the   infiltration carefully, we are   going   to   need   a   notion   of   time.      Recall   that   days   are   divided   into   two   periods: AM, when testing occurs; and   PM, when   contact   occurs.      We   also   have   a   special “initial”   period,   before   the scenario   begins.    This can   be a   bit   unwieldy, so   it’s   better to   have   a   more   uniform   treatment.    Therefore,   we   represent   units of time with   integer values   as follows:
a.          When time = 0, we   are   in   the   initial   period,   also   known   as   day   0.
b.          When time =   1, we are just   after   the   AM   tests   on   day   1.
c.          When time =   2,   we   are just   after the   PM   contacts   on   day   1.   
d.          When time = 3, we   are just   after the   AM   tests   on   day   2.
e.          When time = 4, we   are just   after the   PM   contacts   on   day   2.
f.               And so   forth   …
Accordingly, given d days, we will   have   1   +   2d   time   units.
We’ve   provided some   useful functions to   navigate this   in the   format_list.py   file:
1.          time_of_day   (d,b)   to convert a   day   (integer)   and AM/PM time   (Boolean,   with   True   for   AM   and   False   for   PM)   into one of these time codes   (AM/PM   doesn’t   matter for   day   0).
2.          day_of_time   (t)   to convert a time   unit   into   a   day.
3.          period_of_time   (t)   to convert a time   unit   into an AM/PM   (will   return   AM   for   day   0)
4.          is_initial   (t)   to check whether tis the   initial   period   (i.e.,   0)
5.          str_time   (t)   to convert a   time   period   to   a   string   for   printing,   e.g. “3   (AM)”   (i.e.,   day   3   in   the   morning).   When t = 0 this   returns just “0”   (since day   0   does   not   have   an AM   or   PM).
Your task   is to write the   helpful to   have a   lookup function   contacts_by_time   (participant, time,
contacts_daily).    The first   parameter   is the   name of a   participant, e.g.   “Bella”.    The   second   parameter   is   a      time   unit, e.g. 4   (which   represents day   2   PM).    The third   parameter   is   a   list   of the   contact   groups   on   each   day.      Notice   that the third   parameter   is   indexed   by   day, with day   1   in   index   spot   0;   accordingly,   part   of your   task   is   to   convert   the         time   unit   parameter to the day, and then   adjust to the   list   index.      The   other   part   of   your   task   is   to   search   within   the   contact groups for that day to find the   correct   list for   the   given   participant.      If   the   participant   didn’t   meet   with   anyone on that day, then their   contact   list   is   empty.    As   a   special   case,   contacts   for   day   0   should   also   be   considered   the empty   list for every   participant.    Once you   have   the   correct   list,   return   it.
To   help you test your function, there   is some   code   in main   ()   that   examines the   initial   participant   on   an   early   day,   in
both the AM and   PM   (which should   return the   same   list).      In the   specific   dataset   we’ve   used   so   far, main   ()   will   print   Bella   's contacts for   time   unit   3   (day   2)   are   Bella,   Charlie   and   Edward.
Bella   's contacts for   time   unit   4   (day   2)   are   Bella,   Charlie   and   Edward.
Section   6: Create the   initial vampire   knowledge data structure   and   a   way to   pretty   print   it   (1   mark for correctness +   2   marks for   pretty-printing)
Our    goal    will       be    to      identify    vampires    and      humans      using      logical      deduction   from      data.         We      have      no      interest      in   guesswork and thus   no   interest   in concluding that someone   is probably   a vampire   (or   human);   we   want   certainty.Certainty   is   hard   to   come   by,   but   hard   does   not   mean   impossible.      Over   the   remainder   of   this   assignment,   we   will   explain   some   basic   logical   principles   that justify various deductive steps.      Our goal   in   this   section   is   to   set   up   the   core   vampire knowledge data structure   (“vk structure”) we will   need to   track   the   information   we’ve   learned.Logical   principle   1   :   at a given point in   time   t, reality is binary.      That   is,   every   individual   is   either   a   human   or   a   vampire   at   time   t:   no one can   be   both a   human and   a   vampire   at   the   same   time.      On   the   other   hand,   humanness   is   essentially   a state of grace, and thus   easy   to   lose   over   time   (e.g.,   a   human   at   time   t   can   be   a   vampire   at   time   t   +   1).However,   at   a   given   point   in   time   t,   our   knowledge   about   reality   is   ternary.      At   time   t,   every   individual   has   one   of   three    statuses:    definitely         human       (“   H”),    definitely      vampire    (“V”),    or    unclear      (“   U”).             Here,    definitely    means    with   certainty:   there’s   no   chance   that   a   definite   human   is   “   really”   a   vampire,   or   vice   versa.      This   means that at a specific   moment   in   time   t,   once   H   or   V   status   is   established   for   an   individual,   it   should   never   change   for   that   time   t for that   individual.       Unclear    status    doesn’t    mean    the   individual   is    both   a    human   and   a   vampire   (that’s   impossible!);   it just   means that we aren’t sure.    On   the   other   hand,   as   we   make   deductive   steps,   U   status   might   change   (to “V”   or   “   H”).To   represent   knowledge   at   time   t,   we   use a dictionary where the   keys are   the   participants’   names   and   the   values   are   one   of   three   strings   “   H”,   “V”,   or   “   U”.      Complete   the   function   create_initial_v   k   (participants),   where   participants   is   the   list   of   participants,   and   which   returns   such   a   dictionary   structure.      Initially we   have   no data   about who   is   human and who   is a vampire,   so   everyone’s   initial   status   should   be   unclear   (“   U”).
The   main   ()   function will create   1 +   2d copies   (where d   is   the   number   of   days)   of   the   initial   vk   structure   to   represent   the vampire   knowledge at each   point   in time.      Initially, as   you’ve   created   it,   everyone’s   status   is   unknown   at   all   times.
Complete the function   pretty_print_vampire_knowledge(v   k)   to   print the   results of a vk structure.   Here   is   an   example of what the output should   look   like   on the   initial   vk   structure:
Humans:   (None)
Unclear   individuals: Alice, Angela, Bella, Carlisle,   Charlie,   Edward,
Emmett, Jacob,   Jessica   and   Renee
Vampires:   (None)
Each   row should   be   indented   by two spaces.    Again, text   in   red   should   be   understood to   be   on   a   single   line.      Notice   that format_list(data)   helpfully   returns the string “   (None)   ”   when the given   list   is empty.      Also   notice   that
individuals are alphabetized within the various   lists.
If you do this correctly, main   ()   will   use the function   pretty_print_v   ks   (),   which   in   turn   calls   your
pretty_print_section_6   (), to   print out the   initial vk structures for   each   point   in time   specified   in the   data.


   



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
