# CodeStone-Final-Project
An analysis of the World Happiness Report from 2018 and 2019. Here we analyze 
the differences in various variables which contribute to differences in between
happiness in Western Europe and North America.

The data from this report has been collected from the World Happiness Report
(2018, 2019), which further uses data from the Gallup World Poll. 

To clean this data for use of analyzing regions, we have sorted countries by 
region. Further, we added a categorical variable to compare happiness across
region (detailed further in New Variables). 

## Original Variables

### Overall rank
- Numerical 

Indicating ranking based on over all happiness score.

### Country 
- Categorical 

Name of country.

### Score
- Numerical

Happiness score is a self-reported measure of overall current life satisfaction. This was measured by asking respondents, “Please imagine a ladder, with steps numbered from 0 at the bottom to 10 at the top. The top of the ladder represents the best possible life for you and the bottom of the ladder represents the worst possible life for you. On which step of the ladder would you say you personally feel you stand at this time?” The average of these values represents respective countries.

### GDP per capita
- Numerical

PPP (purchasing power parity) is a rate of conversion which attempts to equalize the purchasing power across all different currencies. The World Happiness Report sources its GDP per capita in PPP values from the 2017 and 2018 World Development Indicators respectively. This value is logged.

### Social support
- Numerical

Social support is a self-reported measure of whether or not the respondent feels they can be helped. Specifically, respondents were asked, “If you were in trouble, do you have relatives or friends you can count on to help you whenever you need them, or not?” and responded with 0 or 1 (no or yes). The average for each respective country creates this value.

### Healthy life expectancy 
- Numerical

Healthy Life expectancy is a measure calculated by comparing the average life expectancy in a given country to the lowest life expectancy of any country. Data was extrapolated from the WHOs health observation data up to 2016. Where missing, life expectancy data for certain countries was found using research and government tools.

### Freedom to make life cohices 
- Numerical

Freedom to make Life Choices is a self-reported measure of whether or not respondents feel they can do what they want with their lives. Respondents were asked, “Are you satisfied or dissatisfied with your freedom to choose what you do with your life?” and responded with 0 or 1 (no or yes). The average for each respective country creates this value.

### Generosity 
- Numerical

Generosity is a measure of whether or not respondents act generously. Respondents were asked, “Have you donated money to a charity in the past month?” and responded with 0 or 1 (no or yes). Generosity is the residual of regressing the national average of this question with GDP.

### Perceptions of Corruption 
- Numerical

Perception of Corruption is a self-reported measure of whether or not respondents feel there is active corruption within government and business. Specifically, respondents were asked, “Is corruption widespread throughout the government or not” and “Is corruption widespread within businesses or not?” and responded to both with 0 or 1 (no or yes). The average for each respective country creates this value. Note: A higher value for this measure represents a lower perception of corruption.

### Year 
- Numerical

Year that the data is from for its respective World Happiness Report.

## New Variables

### Happiness
- Categorical

An IQR-based measure of varying levels of happiness.

### Region
- Categorical

Region of the world. 
