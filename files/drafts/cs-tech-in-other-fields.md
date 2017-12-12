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


### Examples


#### Example 1

I'm a Python fan. I persuade (mostly MATLAB) people around me to use Python. Many people got frustrated at things like the follows and failed to switch.
	
1. There are so many ways to install Python and I feel extremely confused.
1. I never need to update packages in MATLAB; yet now I need to do them in Python.
2. Errors like "XXX package is missing" drives me mad.
3. Jupyter Notebook looks weird compared to my favorite MATLAB IDE.

#### Example 2

One labmate took a machine learning course at CMU. Each assignment had Python and MATLAB version. For one assignment, the starter code of the Python version contained mixed usage of `numpy.ndarray` and `numpy.matrix`; various mysterious "bugs" due to this (poor) mixed usage drove my labmate mad. Despite that Python has essentially won the data science language war over all other ones (MATLAB, R, Julia, etc.), my labmate switched back to MATLAB, which provides a cozy, closed, consistent environment. Essentially, that one poorly written assignment code ruined my labmate's Python experience.


### Reasons





## Understanding "why" is more important than getting things "work".


### Examples