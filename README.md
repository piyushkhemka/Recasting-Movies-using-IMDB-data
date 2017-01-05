# Problem Statement

Given an input movie, can we suggest a suitable replacement for the lead actor male and lead actor female, if the movie were to be remade in the year specified by the user.
Example questions answered by the model:

1. Given the movie - ’Inception’, who would be the best actor to play the lead role, if the movie was to be made in 1950s?
2. Given the movie - ’Titanic’, who would be the best actor to play Kate Winslet’s role, if the movie was to be made in 2016?
3. Who would play Arnold Schwarzenegger’s role in Terminator if the movie was to be made in 1940s or if it was made today?




## Results
------
#### Quantative Results
Following are the results from the 3 models which we tested -


|  Distance Function  | Male Dataset Accuracy  | Female Dataset Accuracy  |
|--:|--:|--:|
|  Cosine | 44.62%  |  61.97% |
|  Manhattan |  41. 39% | 49.47%  |
|  Euclidean | 43.54%  |  51.04% |
 
#### Testing Methodology
Quantative: For any given remake we ran our model for the actor who appeared in the original movie and let our model predict possible replacements for him. We let our model come up with multiple (5% of the dataset size) replacements for the original actor. If the set of replacement actors contained the actor who actually appeared in the remake we call that a ’hit’ for our model. We counted for what percentage of remakes our model was ’hit’. We did this test for both actors as well as actresses.



 
#### Qualitative results:


| Lead Actor of Inception(2010) if it was remade in 1960|
|--:|
|Marlon Brando|
| Paul Newman  |
|  Robert Duvall |
| James Garner  |
|  Richard Burton |
-----
| Lead Actor of Its a Wonderful life(1946) if it was remade in 2016  |
|--:|
|Matt Damon|
|Adrien Brody |
|Matthew McConaughey|
|James Franco|
| Will Smith |


Testing replacements for an older male actor <br>Remake Lord of the Rings (2001) in 2011 
<br>
Top 5 replacements for Ian Mckellen
- Bill Nighy
- Liam Neeson
- John Goodman 
- Bob Hoskins
- Jeff Daniels

Testing for lead male actor - James Bond <br>
Remake Die Another Day(2000) in 1980<br> 
Top 5 replacements for Pierce Brosnan -
- Roger Moore 
- Sean Connery
- Harrison Ford
- Robert Redford 
- Clint Eastwood


Testing for lead female actor in 90s <br>
Remake Mr. & Mrs Smith (2005) in 1990 <br>
Top 5 replacements for Angelina Jolie.
- Nicole Kidman 
- Julia Roberts 
- Cate Blanchett 
- Jodie Foster
- Sharon Stone

Testing for lead female actor today<br> Remake Mr. & Mrs Smith (2005) in 2016 <br>
Top 5 replacements for Angelina Jolie.

- Keira Knightley 
- Natalie Portman 
- Jessica Chastan 
- Anne Hathaway 
- Kirsten Dunst

Testing lead female actor in 60s<br>
Recast Kate Winslet in Titanic from 1998 to 1960
- Maggie Smith
- Glenda Jackson
- Joanne Woodward
- Grace Kelly
- Judi Dench


Recast Older Actress<br>
Replacing Meryl Streep in The Devil wears Prada (2006) to 2016
- Jessica Lange
- Sissy Spacek
- Holly Hunter
- Jodie Foster
- Emma Thompson


Child Actor test<br>
Remake Home Alone 1990 in 2001 <br>Replace Macaulay Culkin
- Taylor Lautner 
- Daniel Radcliffe 
- Dylan O Brien
- Dev Patel
- Logan Lerman

#### Testing Methodology
Qualitative: Intuitively how good the top 5 replacements for any actor are for any given movie. 


(More details of how we arrived at these results in the proposal)
##
##### ** Code available on Request. The git repo contains the initial proposal, progress and final report

##
##
