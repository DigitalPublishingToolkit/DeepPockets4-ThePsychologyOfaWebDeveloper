---
Pr-id: MoneyLab
P-id: INC Reader
A-id: 10
Type: article
Book-type: anthology
Anthology item: article
Item-id: unique no.
Article-title: title of the article
Article-status: accepted
Author: name(s) of author(s)
Author-email:   corresponding address
Author-bio:  about the author
Abstract:   short description of the article (100 words)
Keywords:   50 keywords for search and indexing
Rights: CC BY-NC 4.0
...


# Post-Wordpress Web-dev, Fuck It.

Psst, it’s me. Your Post-WordPress web developer. Yeah, I’ll tell you a
bit more about my story.

<center>*\*(intro) What did the subject look like as a healthy and normal person?\**</center>

It all started the day I created my first social media account. Having
an account brought along with it the possibility to fill up my gallery
with personal pictures, select and list top friends on one’s profile,
and fill in the lists asking about one’s favorite movies, foods, and
miscellaneous interests.

Nothing was blank on my Hi5 (Balkan Myspace) profile. I was crafting and
re-crafting it daily. My favorite part was customizing the wallpaper
through copying codes from other platforms in the platform’s hypertext
boxes. I went through many different kinds of wallpapers: from clouds to
black and white skate parks during sunset. Once I entered my
‘pitch-black phase’, I focused more on the quality of my lists and made
sure they showed some good taste.

Styling one’s profile was the most enjoyable part of my user’s
experience. Profiles were exchanged amongst users as exemplary
references to look at while building one’s own.

Today, I can’t tell if enabling the users to apply aesthetic changes on
social media platforms (which were ultimately designed for user
connection) was a deliberate aspect of the platform’s design, but I do
believe this was the reason why the switch to the currently most
dominant one (Facebook), a platform where aesthetic customization is
*disabled*, was so easy.

Between this moment of stylizing my wallpapers in 2009 and my
bureaucratic situation in 2019 lies a huge gap in my coding practice.
Attending the bootcamp school bridged this gap: I started building
websites from scratch, not just inserting codes on someone else’s
platform.

The first few small-scale websites I built were handmade—meaning they
were built with HTML, CSS, and Javascript; basic tools for building any
kind of website. Learning how to build a button, for example, already
made me realize that the design of this button can rather easily
manipulate the user’s mood, akin to how a doorknob of a random door
would. Where does the door lead to? Is it locked? What’s lurking on the
other side? Should I *open* the door? Multiple, diverse types of buttons
leading to a manifold of pages made me wonder about the amount of space
a website occupies within various digital infrastructures.

> *\*(rising action) Which software affected the subject’s condition?\**

At the time when I started building websites for clients, WordPress was
the go-to software to use in order to get a sense of the server-client
traffic behind a website. In the beginning, I charged very little and
said yes to any project or deadline. The projects were simple; the
deadlines extremely tight.

Because I felt rushed, I used theme-building helpers (such as Divi) to
meet the client’s expectations in time. The design would highly depend
on the limitations and freedoms of the software’s given functionalities:
using theme builders that had an easy drag-and-drop functionality to
create the looks of a digital space constrained my creative output. The
limited possibilities these builders provided was not satisfying enough
to feel creatively fulfilling to someone who wanted to break out of the
default grids and blocks, a.k.a: me. Not *seeing* the code that built my
decisions felt weird.

After I built two websites with extra builder products, I felt like a
scam to the world of web development. I felt like *any*body could do it
and that *every*body was doing it. As I was claiming the title of a web
developer, I felt like I had to live up to it. But also, I just really
liked coding. So I started picking up on PHP language and coding custom
themes, after which I finally started feeling like a real web developer
(whatever that means).

Identifying myself with this expert software in the company of other web
developers made me feel quite shy at first, but upon discovering that
the majority of web infrastructure is built with this same software at
some point started making me feel average.

As I was building websites, it seemed to me that the software was
updating itself according to the user’s needs really fast, and that
whatever users lacked in their editing freedom soon became an option in
a plug-in library: a true catering to their needs. It is true that
WordPress software updates not only grow alongside the needs of its
user, but also follow the web developer’s imagination, which, when
turned into a plug-in, can be uploaded to the WordPress Plug-in library.
That’s what open-source means; contributors add themes and plug-ins to
it, for software improvement. ‘All technology reflects the society that
produces it, including its power structures and prejudices.’ — Douglas
Rushkoff, *Program or be Programmed*.

I don’t know if being content with theory justifying my software choice
was naive, but I was having fun. I was entertained by the underlying
irony of the previously explained WordPress cringe.

> *\*(climax) How did the subject liberate oneself from the software’s
> constraints?\**

That’s when I became a Post-WordPress web developer. As a Post-WordPress
web developer, I knew what I *didn’t* want from my coding endeavors:
plug-ins (unless custom-coded), hamburger menu (unless absolutely
necessary), WP default styling (a.k.a. classification and names
according to the semantics), a deadline within the month, and having to
say yes to the reducing amount of pages as well as meeting the client
once a week. I wanted to make rules that would bring me closer to
building *light* websites at a *slow* pace—what my friend Clara calls
‘handmade coding’.

With handmade coding, I could build a website like I’d imagined building
a space back in the days of studying architecture: hand in hand with the
inhabitant or citizen, the user, and their individual taste. Our
collaboration would mean meeting and building each other’s differences,
on whatever interface necessary.[^16postwordpresswebdevfuckit_1]

The *post* in my title refers to the fact that even though I am aware of
the WordPress cringe, it’s the tool I choose to operate with despite its
reputation. That in my productivity I have found liberation, not
software enslavement; that WordPress will succumb to my needs and
accommodate the skills necessary for me to have whilst collaborating
with my client.

Here comes an example of my liberation. The following code was written
for the client’s portfolio website and in agreement with the client:

####&lt;details&gt;

####&emsp; &lt;summary style="margin-left: 50%"&gt;editor&lt;/summary&gt;

####&emsp; &lt;?php \$loop = new WP\_Query( array( 'post\_type' =&gt; 'editor',
&emsp; 'posts\_per\_page' =&gt; 10 ) );


####&emsp; if ( \$loop-&gt;have\_posts() ):

####&emsp;&emsp; while ( \$loop-&gt;have\_posts() ) : \$loop-&gt;the\_post();

####&emsp;&emsp; ?&gt;

####&emsp;&emsp; &lt;details class="secondary-details"&gt;

####&emsp;&emsp; &lt;summary class="project" id="editor-project"

####&emsp;&emsp; onclick="editorProjectTop()"&gt;&lt;?php the\_title('⊃&nbsp;');

####&emsp; ?&gt;&lt;/summary&gt;

####&emsp;&emsp;&emsp; &lt;div class="entry-content"&gt;

####&emsp;&emsp;&emsp;&emsp; &lt;?php the\_content(); ?&gt;

####&emsp;&emsp;&emsp; &lt;/div&gt;

####&emsp;&emsp;&emsp; &lt;div class="mode-buttons"&gt;

####&emsp;&emsp;&emsp;&emsp; &lt;button class="feel-btn" onclick="editorProjectTop()"&gt;see, hear,&emsp; sense&lt;/button&gt;

####&emsp;&emsp;&emsp;&emsp; &lt;button class="read-btn"

####&emsp; onclick="editorProjectTop()"&gt;read&lt;/button&gt;

####&emsp;&emsp;&emsp; &lt;/div&gt;

####&emsp;&emsp; &lt;/details&gt;

####&emsp; &lt;?php endwhile;


####&emsp; else: ?&gt;

####&emsp;&emsp; &lt;p&gt;&lt;?php echo '&lt;div&emsp; class=“void"&gt;&lt;/div&gt;’;?&gt;&lt;/p&gt;

####&emsp; &lt;?php endif;


####&emsp; wp\_reset\_query();

####&emsp; ?&gt;

####&lt;/details&gt;

The code indicates that there is a button called ‘editor’ on the
website, which is one of the professional roles that define the client’s
professional history. Clicking on this button opens a list of project
titles (‘secondary-details’) in which this role is played out. Each
project (‘editor-project’) is also clickable and when clicked opens the
content (‘entry-content’) the client added to it in the admin panel of
the website.

Content is divided between two reading modes: visual and textual. By
default, textual content opens on the first click. Once you reach the
end of the content, there is a button that switches between two reading
modes (‘feel-btn’ and ‘read-btn’, *btn* being button). If there are no
projects assigned to this role, one can choose to show void (‘void’). A
void, in my collaboration with this respective client, was represented
by a dark blue circle piercing the soft aesthetics of the website. In a
nutshell: handmade coding of a fairly light website.

The code explained here is my favorite code written thus far. It
speculates on the client’s future, doesn’t limit it to one professional
role, nor demands the existing roles to be filled with more professional
activities. It was written with the purpose to emphasise the uncertainty
any professional role might have. These professional roles could fade
out and turn into the designed void (dark blue circle), or they could be
emphasized more and be accompanied by other projects in the future.

After passing two interviews for the ‘creative developer’ role at
WeTransfer in 2021, I was invited to work on a technical assignment. The
challenge was to code a ‘whack-a-mole’ game through which the company
could get a sense of my creativity level. There was no framework,
language, tool or imagination requirements, but there was one big ask:
not to spend too much time on the task. In the span of the single week I
was given to develop it, I spent a total of nine hours on it.

Adding to this, I must say my creativity depends on other people. I
found and copy-pasted the simplest HTML/CSS/Javascript code of a
whack-a-mole (by Ania Kubów) and decided to change the code according to
my friends’ answers to the question: *If you could whack one thing for
the rest of your life, what would it be?*

One of the answers was Facebook:

####&lt;body&gt;

####&emsp;&lt;header&gt;

####&emsp;&emsp;&lt;div class="display-flex"&gt;

####&emsp;&emsp;&emsp;&lt;p&gt;Facebook killed:&lt;/p&gt;

####&emsp;&emsp;&emsp;&lt;p id="score"&gt;0&lt;/p&gt;&lt;p&gt; times.&lt;/p&gt;

####&emsp;&emsp;&lt;/div&gt;

####&emsp;&emsp;&lt;div class="display-flex"&gt;

####&emsp;&emsp;&emsp;&lt;p&gt;Time Left:&lt;/p&gt;

####&emsp;&emsp;&emsp;&lt;p id="time-left"&gt;666&lt;/p&gt;

####&emsp;&emsp;&lt;/div&gt;

####&emsp;&lt;/header&gt;

####&emsp;&lt;div class="grid"&gt;

####&emsp;&emsp;&lt;div id="1" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="2" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="3" class="square facebook"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="4" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="5" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="6" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="7" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="8" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="9" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="10" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="11" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="12" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="13" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="14" class="square"&gt;&lt;/div&gt;

####&emsp;&emsp;&lt;div id="15" class="square"&gt;&lt;/div&gt;

####&emsp;&lt;/div&gt;


####&emsp;&lt;footer&gt;

####&emsp;&emsp;&lt;p&gt;

####&emsp;&emsp;&emsp;\[person\] undoubtedly wants to whack Facebook all the time, and for a long time. &lt;br&gt;

####&emsp;&emsp;&emsp;Is your name not \[person\] &lt;a href="/index.html"&gt;My name is not \[person\].&lt;/a&gt;&lt;/p&gt;

####&emsp;&lt;/footer&gt;

####&lt;/body&gt;

This is the body of a web page that was built to show the score (how
many times Facebook was whacked); above it one can see the countdown
time. Underneath this, a grid of fifteen squares floats in which the
logo of Facebook appears randomly, and which the user is expected to
click or shoot. The footer of the page asks if the user’s name is
\[person\]’s name, a.k.a. if they wish to be someone else while whacking
this evil, Zuckerberg-spawn thing.

The code was adjusted to the \[person\]’s specific desires in whacking
Facebook, which was done in the following ways: even though the timer’s
countdown started counting down from 666 seconds, there was, if desired,
additional time given for completion of the mission (1,000 seconds).
Next to this, the Facebook logo would hang around in one of the grid’s
squares, long enough to shoot it. It was rather impossible to miss.
Unfortunately, the message at the end of the countdown reminds the user
that, despite their astonishing scores, Facebook still exists.

####function countDown() {

####&emsp;currentTime--

####&emsp;timeLeft.textContent = currentTime

####&emsp;if (currentTime == 0) {

####&emsp;&emsp;clearInterval(countDownTimerId)

####&emsp;&emsp;clearInterval(timerId)

####&emsp;&emsp;alert('There is no time left to whack Facebook. Despite your score of: '+ result + ' points, Facebook still exists.')

####&emsp;}

####}

####let countDownTimerId = setInterval(countDown, 1,000)

I furthermore collected eight answers from my peers to the question
*What would you whack?* The results were: a lack of confidence, eczema,
architecture (i.e. one school building per day), sea creatures, Gerald
Darmanin, applications and/or funding opportunities, and ‘I would whack
people who think that rationality is better than emotions and
intuitions; I would whack everyone who expects and forces me to be
“clear” according to *their* understanding of clarity; I would whack the
idea that if you make work you have to be able to write about it; I
would whack people who tell me what to do and how to do things without
me asking for it; I would whack people who say that they would never
drink their own pee if they were in the desert almost dying. *Liars.*’

I loved turning the project into research about what my peers would
whack and discovering if my coded reflections on their wishes could get
me hired for my creativity level. During the interview with a front-end
web developer at WeTransfer, I was told that I was *sooo very* creative.

You can find out the answer to the question whether I got the job or not
by reading the following ‘list’ of websites I dream of building, yet
never have the time to:

####&emsp;&lt;a href="https://whack-what.vercel.app/"&gt;This was a technical assignment for WeTransfer, but I didn't get the job.&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="/instagram-poetry/ig\_bore.html"&gt;IG bore&lt;/a&gt;&lt;br&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;Click here to stop scrolling&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;Blue Heart Agency&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;I Just Wanna&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;Button Poetry&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;The Writer is Present&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;We only got 10 mins to save the content&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;Mute everything&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;Forever load, but not like that&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;Rotating structures, floating points, and similar&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;All known blanks&lt;/a&gt;&lt;br&gt;

####&emsp;&lt;a href="\#"&gt;Working station of profile production&lt;/a&gt;&lt;br&gt;

It’s not a list in code. Were I to write semantic code, it’d be wrapped
in a &lt;ul&gt;&lt;/ul&gt; tag, followed by a &lt;li&gt; tag around each
&lt;a&gt; tag. Then I’d get rid of the line break tags (&lt;br&gt;). The
way this list looks like right now doesn’t bother me in the slightest.
Any web developer inspecting it might find these codes very simple,
because they *are*. And they bring me a lot of joy.

[^16postwordpresswebdevfuckit_1]: [*https://motherfuckingwebsite.com/*](https://motherfuckingwebsite.com/)
