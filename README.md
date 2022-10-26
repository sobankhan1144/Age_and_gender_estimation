# Age_and_gender_estimation
Age and Gender estimation on public dataset including wiki_imdb and FGnet
All supporting files availabel in google drive link provided [here](https://drive.google.com/file/d/19zwMs4J41QyyAZgu-Cwgi2t3I2GUFxpi/view?usp=sharing)

Age grouping can be adjusted in the notebook according to your liking 
```
def age_group(age):
    if age >=0 and age <=2:
        return 0
    elif age >2 and age <=5:
        return 1
    elif age >5 and age <=13:
        return 2
    elif age >13 and age <=18:
        return 3
    elif age >18 and age <=24:
        return 4
    elif age >24 and age <=33:
        return 5
    elif age >33 and age <=48:
        return 6
    elif age >48 and age <=64:
        return 7
    else:
        return 8
```
