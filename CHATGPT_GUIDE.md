# ChatGPT Integration Guide

This guide provides specific instructions for using the entertainment ratings with ChatGPT.

## Quick Start

1. Start a new ChatGPT conversation
2. Upload `entertainment_ratings.csv` or `entertainment_ratings.xlsx`
3. Use one of the prompt templates below

## Prompt Templates

### For Individual Recommendations

**For Sky:**
```
Based on Sky's ratings and favorites in the uploaded file, please recommend:
- 5 new movies I might enjoy
- 3 TV shows to watch next
- 2 music artists to explore

Consider that favorites (marked TRUE) are especially important preferences.
```

**For Tay:**
```
Looking at Tay's preferences in the uploaded data:
- What are the top genres Tay prefers?
- Recommend 5 new entries based on their favorites and high ratings
- Are there any patterns in their rating preferences?
```

### For Shared Recommendations

**Date Night:**
```
Based on both Sky and Tay's ratings, suggest movies that:
- Both rated 8.0 or higher
- Match genres they both enjoy
- Would make great viewing together

Please explain why each recommendation fits both preferences.
```

**Discover Together:**
```
Find common ground between Sky and Tay:
- Which genres do they both enjoy?
- What items did they both rate highly?
- Recommend new content that matches their shared interests
```

### For Analysis

**Rating Analysis:**
```
Analyze the rating patterns in this data:
- What's the average rating for each person?
- Which categories (Movie/TV/Music) does each person rate higher?
- Where do their tastes align or differ the most?
```

**Recommendation Engine:**
```
Act as a recommendation engine:
- For each person, identify their top 3 favorite genres
- Based on their favorites, predict what they might rate 9.0 or higher
- Suggest specific titles with reasoning

Use the "favorite" flag as the strongest signal, then high ratings, then genre patterns.
```

## Advanced Usage

### Filtering Recommendations

```
Recommend 5 movies for Sky that are:
- Sci-Fi genre (based on their high ratings in this genre)
- NOT already in the list
- Released after 2010
- Similar to their marked favorites

Explain each recommendation based on the data patterns.
```

### Comparative Analysis

```
Compare Sky and Tay's preferences:
- Create a compatibility score for different genres
- Identify what they disagree on most
- Find hidden gems one person loved but the other hasn't rated highly
- Suggest items where they might want to give another chance
```

### Creating New Lists

```
Based on this data, create a "Must Watch Together" list:
- 10 items (mix of movies and TV shows)
- Items both people would rate 8.5+
- Prioritize favorites
- Include variety across genres

Format as a ranked list with explanations.
```

## Tips for Better Recommendations

1. **Be Specific**: Mention which person's preferences should be prioritized
2. **Use Favorites**: Reference the "favorite" flags for more weighted recommendations
3. **Consider Context**: Mention mood, occasion, or specific criteria
4. **Ask Follow-ups**: Refine recommendations based on the initial suggestions

## Data Interpretation

### Rating Scale
- **9.0-10.0**: Absolute favorites, highly rewatch/relisten
- **8.0-8.9**: Really enjoyed, would recommend
- **7.0-7.9**: Liked it, good but not great
- **Below 7.0**: Okay or didn't enjoy

### Favorite Flag
- **TRUE**: Extra weight in recommendations (2x importance)
- **FALSE**: Standard rating weight

## Example Conversation Flow

```
You: [Upload entertainment_ratings.csv]

You: "Based on Sky's favorites, what should they watch next?"

ChatGPT: [Analyzes Sky's favorites: Breaking Bad, Inception, The Matrix, 
The Beatles, Radiohead, Pink Floyd. Notices preference for mind-bending 
sci-fi and classic rock]

ChatGPT: "Based on Sky's preferences, I recommend:
1. Dark (TV Show) - Complex sci-fi like Inception
2. Blade Runner 2049 (Movie) - Matches Matrix and Inception style
3. Led Zeppelin (Music) - Similar to Pink Floyd and classic rock favorites
..."

You: "Now find something both Sky and Tay would enjoy watching together"

ChatGPT: [Identifies overlap - both loved Breaking Bad and Stranger Things]

ChatGPT: "For both of you, I suggest:
1. Better Call Saul - Both rated Breaking Bad as favorite
2. The Witcher - Fantasy like Game of Thrones which Tay favored
..."
```

## Updating the Data

After watching/listening to new content:

1. Add new rows to the CSV/Excel file
2. Re-upload to ChatGPT in the same conversation
3. Ask: "Based on these new ratings, update your recommendations"

## Privacy Note

The ratings data stays in your ChatGPT conversation and is not shared publicly. Each conversation is independent - start fresh or continue previous conversations as needed.