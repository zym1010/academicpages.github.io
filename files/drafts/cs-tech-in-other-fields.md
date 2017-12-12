# thoughts on applying CS tech to other fields

This is a summary of difficulties in applying CS technologies in other sci&tech fields, such as neuroscience and biology.

## A link to the past

When faced with some new thing, **everybody** wants to draw on their experience of old things similar to it in order to understand it. This is **particularly** the case for non-CS people in the face of CS products (you can replace CS with any other field).

### Examples

#### Example 1

I wrote a tool for data management in the lab before ([DataSMART](https://github.com/leelabcnbc/datasmart/)). The options for some data pipeline operations are specified using JSON files, which is a very simple format for document-type data. Some people around me feel JSON is intimidating and strange to them, and ask me if they can specify options in MATLAB.

I guess it's fine to specify options using, say, MATLAB `struct`, but I really feel MATLAB `struct` and JSON are no different, and JSON is probably better.

#### Example 2

I have advocated lab people to upload their reports to GitHub so that everybody knows what is going on of everybody else. Some people in the lab prefer to write reports in Word/LaTeX. Although I told them many times that Jupyter Notebook can handle image, text, math, code all in one, they simply won't budge.


### Reasons

Imagine that there is a graph of CS tools and concepts in your brain. The graph of a non-CS person should look very different from that of a CS-person (well you can replace CS with almost any other thing).

For example 1, CS people might treat both MATLAB `struct` and JSON as data formats that can (in Python terminology) store arrays, dictionaries, etc, and non-CS people might simply treat them as separate things.

````
For CS people:

[JSON] --- [MATLAB struct]
   \                /
    \              /
     \            /
      [Python dict] 
      
For non-CS people:

[JSON]     [MATLAB struct]
                     
                    
                   
      [Python dict]

````

For example 2, non-CS people might associate Jupyter Notebook with Python, which is not very popular in my field (neuroscience), and Python has worse user experience than MATLAB, in terms of installation, debugging, etc. Overall, non-CS people might switching to Jupyter will let them cost more, as the its convenience is overwhelmed by all the (potential) headaches for setting it up. In addition, they may feel worried that they need to learn Markdown. CS people might consider all those headaches to be minor, learn Markdown in no time if not already learned, and focus on the convenience of having text and code together. 

````
For CS people:

      [LaTeX] --------[Markup Languages]
      /                   /     |
     /                   /      |
    /                   /       |
   /                   /        |
[Jupyter] --- [Markdown]      [HTML] 
   \                
    \              
     \            
  [Python]   
      
For non-CS people:

      [LaTeX] 
      /                       
     /       
    /         
   /          
[Jupyter] --- [Markdown]      [HTML] 
   \                
    \              
     \            
  [Python] --- [Difficult to install]

````


Essentially, CS people have deeper understandings of CS products and have better tolerance of those headaches in a layman's opinion.

[A very good explanation on the difference between pro users and normal users](https://www.zhihu.com/question/21261475/answer/17723291). It should apply to CS people vs. non-CS people as well.



## First impression and ease of deployment is extremely important.

Leaving people a good impression is very important, and it's particular important for selling a product in domain A to people in domain B.

### Examples


#### Example 1

I'm a Python fan. I persuade (mostly MATLAB) people around me to use Python. Many people got frustrated at things like the follows and failed to switch.
	
1. There are so many ways to install Python and I feel extremely confused.
1. I never need to update packages in MATLAB; yet now I need to do them in Python.
2. Errors like "XXX package is missing" drives me mad.
3. Jupyter Notebook running in a browser looks weird compared to my favorite MATLAB IDE.

#### Example 2

One labmate took a machine learning course at CMU. Each assignment had Python and MATLAB version. For one assignment, the starter code of the Python version contained mixed usage of `numpy.ndarray` and `numpy.matrix`; various mysterious "bugs" due to this (poor) mixed usage drove my labmate mad. Despite that Python has essentially won the data science language war over all other ones (MATLAB, R, Julia, etc.), my labmate switched back to MATLAB, which provides a cozy, closed, consistent environment. Essentially, that one poorly written assignment code ruined my labmate's Python experience.


### Reasons

Again, it's due to that people organize CS concepts in their mind differently, they estimate the costs of handling new concepts and difficulties differently.

In example 1, CS people who have experience with C++ or any other lower-level languages will not find installing and updating packages to be very annoying, as they have struggled with such issue for many times; non-CS people who are familiar with MATLAB will find such issues unacceptable.

In example 2, CS people know more that there are well written programs and badly written ones---any great language can be used in bad ways; non-CS people may unconsciously will evaluate a language purely based on some of their own (highly biased) specific use cases.


## Understanding "why" is more important than getting things "work".

I think this is a problem specific to deep learning. In the deep learning era, people have developed many models that "work", without knowing why they work. This is an issue recognized by almost every deep learning professional.

On the other hand, I feel the issue of "why" is highly valued by many scientific fields. In neuroscience, if a paper does not have a section on "why" a model works, then the chance of publication will be slim. 


## User interface has to be really friendly and intuitive.

As a CS person, I am OK with struggling with mysterious bugs of open-source programs. I think as CS people understand the underlying mechanisms of those programs better, they are more proactive in fixing bugs, and can often find the correct way to solve them quickly.

For example, if a program gives some mysterious error, I will typically copy and paste that error information into Google, see what other people are saying, and figure out the correct solution for me out of a lot of noisy and misleading ones. If googling doesn't work, I will try to check source code, set break point somewhere, add some print statements, etc. to figure out what's going on.

Non-CS people won't do any of these. They will check user documentation at most, which will never contain what they want to solve the error, and get stuck and frustrated.

Essentially, I feel selling CS products to non-CS people is like selling cars to average customers without knowledge of automobile mechanics. Many CS products are just not that reliable and not worth money and time, if we treat CS product as cars that are simply expected to work, without any customer's help.
