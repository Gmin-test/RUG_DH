# Game of Thrones
All the files and contents are from [kaggle](https://www.kaggle.com/datasets/mylesoneill/game-of-thrones/). The repository is just for practice on how to use Github.
## About Dataset
This dataset combines three sources of data, all of which are based on information from the book series.
1. **battles.csv** which contains Chris Albon's "The War of the Five Kings" Dataset. Its agreat collection of all of the battles in the series.
   
| Header                 | Description                                   | Data Type  |
|------------------------|-----------------------------------------------|------------|
| Name                   | Name of the battle                            | Text       |
| Year                   | Year of the battle                            | Integer    |
| Battle Number          | Unique identifier for the battle              | Integer    |
| Attacker King          | King leading the attacking side               | Text       |
| Defender King          | King leading the defending side               | Text       |
| Attacker 1             | Primary attacking house/faction              | Text       |
| Attacker 2             | Additional attacking house/faction            | Text       |
| Attacker 3             | Additional attacking house/faction            | Text       |
| Attacker 4             | Additional attacking house/faction            | Text       |
| Defender 1             | Primary defending house/faction              | Text       |
| Defender 2             | Additional defending house/faction            | Text       |
| Defender 3             | Additional defending house/faction            | Text       |
| Defender 4             | Additional defending house/faction            | Text       |
| Attacker Outcome       | Outcome for the attacking side (win/loss)    | Text       |
| Battle Type            | Type of battle (e.g., pitched battle)        | Text       |
| Major Death            | Whether a major character died (1 for true, 0 for false) | Boolean   |
| Major Capture          | Whether a major character was captured (1 for true, 0 for false) | Boolean   |
| Attacker Size          | Size of the attacking force                  | Integer    |
| Defender Size          | Size of the defending force                  | Integer    |
| Attacker Commander     | Main commander of the attacking side         | Text       |
| Defender Commander     | Main commander of the defending side         | Text       |
| Summer                 | Whether the battle occurred in summer (1 for true, 0 for false) | Boolean   |
| Location               | Location where the battle took place         | Text       |
| Region                 | Region where the battle occurred             | Text       |
| Note                   | Additional notes or information about the battle | Text       |

2. **character-deaths.csv** from Erin Pierce and Ben Kahle. This dataset was created as a part of their Bayesian Survival Analysis.

| Header               | Description                             | Data Type  |
|----------------------|-----------------------------------------|------------|
| Name                 | Character's name                        | Text       |
| Allegiances          | House or group the character is aligned with | Text     |
| Death Year           | Year of the character's death (if applicable) | Integer |
| Book of Death        | Book in which the character dies         | Integer    |
| Death Chapter        | Chapter in which the character dies      | Text       |
| Book Intro Chapter   | Chapter in which the character is introduced | Text    |
| Gender               | Gender of the character                  | Text       |
| Nobility             | Whether the character is of nobility (1 for true, 0 for false) | Boolean |
| GoT                  | Whether the character appears in "Game of Thrones" (1 for true, 0 for false) | Boolean |
| CoK                  | Whether the character appears in "A Clash of Kings" (1 for true, 0 for false) | Boolean |
| SoS                  | Whether the character appears in "A Storm of Swords" (1 for true, 0 for false) | Boolean |
| FfC                  | Whether the character appears in "A Feast for Crows" (1 for true, 0 for false) | Boolean |
| DwD                  | Whether the character appears in "A Dance with Dragons" (1 for true, 0 for false) | Boolean |

3.  **character-predictions.csv** includes their predictions on which character will die.
   
| Header               | Description                                       | Data Type  |
|----------------------|---------------------------------------------------|------------|
| S.No                 | Serial number for identification                   | Integer    |
| actual               | Actual status (0 for false, 1 for true)            | Integer    |
| pred                 | Predicted status (0 for false, 1 for true)         | Integer    |
| alive                | Probability of being alive                        | Float      |
| plod                 | Probability of being dead                         | Float      |
| Name                 | Character's name                                  | Text       |
| Title                | Character's title or honorific                    | Text       |
| Male                 | Gender of the character (1 for true, 0 for false) | Integer    |
| Culture              | Cultural background of the character              | Text       |
| Date of Birth        | Character's date of birth                         | Text       |
| Date of Death        | Character's date of death (if applicable)         | Text       |
| Mother               | Character's mother                                | Text       |
| Father               | Character's father                                | Text       |
| Heir                 | Character's heir                                  | Text       |
| House                | Character's house or affiliation                  | Text       |
| Spouse               | Character's spouse                                | Text       |
| Book 1               | Appears in Book 1 (1 for true, 0 for false)       | Integer    |
| Book 2               | Appears in Book 2 (1 for true, 0 for false)       | Integer    |
| Book 3               | Appears in Book 3 (1 for true, 0 for false)       | Integer    |
| Book 4               | Appears in Book 4 (1 for true, 0 for false)       | Integer    |
| Book 5               | Appears in Book 5 (1 for true, 0 for false)       | Integer    |
| Is Alive Mother      | Mother's current status (1 for true, 0 for false) | Integer    |
| Is Alive Father      | Father's current status (1 for true, 0 for false) | Integer    |
| Is Alive Heir        | Heir's current status (1 for true, 0 for false)   | Integer    |
| Is Alive Spouse      | Spouse's current status (1 for true, 0 for false) | Integer    |
| Is Married           | Marital status (1 for true, 0 for false)          | Integer    |
| Is Noble             | Nobility status (1 for true, 0 for false)         | Integer    |
| Age                  | Character's age                                   | Integer    |
| Number of Dead Relations | Count of dead relations                         | Integer    |
| Boolean Dead Relations | Boolean value indicating if there are dead relations (1 for true, 0 for false) | Integer    |
| Is Popular           | Popularity status (1 for true, 0 for false)      | Integer    |
| Popularity           | Popularity score                                  | Float      |
| Is Alive             | Overall alive status (1 for true, 0 for false)    | Integer    |

## Acknowledgements
Firstly, there is battles.csv which contains Chris Albon's "The
War of the Five Kings" Dataset, which can be found here:
https://github.com/chrisalbon/war_of_the_five_kings_dataset . Its a
great collection of all of the battles in the series.

Secondly we have character-deaths.csv from Erin Pierce and Ben
Kahle. This dataset was created as a part of their Bayesian Survival
Analysis which can be found here:
http://allendowney.blogspot.com/2015/03/bayesian-survival-analysis-for-game-of.html

Finally we have a more comprehensive character dataset with
character-predictions.csv. This comes from the team at A Song of Ice and Data who scraped it from http://awoiaf.westeros.org/ . It
also includes their predictions on which character will die, the
methodology of which can be found here:
https://got.show/machine-learning-algorithm-predicts-death-game-of-thrones
