# Age_and_gender_estimation
Age and Gender estimation on public dataset including wiki_imdb and FGnet
All supporting files availabel in google drive link provided [here](https://drive.google.com/file/d/19zwMs4J41QyyAZgu-Cwgi2t3I2GUFxpi/view?usp=sharing)

- Age grouping can be adjusted in the notebook according to your liking 
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

- Also change the dataset file paths accordingly in code here

```
train_df = pd.read_csv('/content/utk_final.csv') # for fgnet "/content/fgnet_with_age_groups.csv" 
train_df['final_label'] = train_df['final_label'].astype(str)
test_df = pd.read_csv('/content/fgnet_final_file.csv') # for fgnet "/content/fgnet_with_age_groups.csv" 
test_df['final_label'] = test_df['final_label'].astype(str)
```
