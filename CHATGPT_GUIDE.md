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

**For Landen:**
```
Analyze Landen's ratings and favorites to:
- Identify their preferred genres and rating patterns
- Recommend 3 movies, 2 TV shows, and 2 music artists
- Consider both their individual ratings and favorites
```

**For Hanna:**
```
Based on Hanna's preferences in the data:
- What types of content do they rate highest?
- Recommend recent releases (post-2015) they might enjoy
- Focus on items marked as their favorites for similar recommendations
```

### For Shared Recommendations

**Group Movie Night:**
```
Based on all four people's ratings (Sky, Tay, Landen, Hanna), suggest movies that:
- Everyone rated 7.5 or higher
- Match genres that most people enjoy
- Would make great group viewing

Please explain why each recommendation works for the group.
```

**Discover Together:**
```
Find common ground among all four people:
- Which genres do they all enjoy?
- What items did most people rate highly?
- Recommend new content that matches their shared interests
- Identify the "consensus favorites" that multiple people marked as TRUE
```

**Couple Recommendations:**
```
For Sky and Tay specifically, or Landen and Hanna:
- Find movies both people rated 8.0+
- Suggest content based on overlapping favorites
- Consider their combined genre preferences
```

**Platform-Based Recommendations:**
```
Based on the streaming platforms in the uploaded data:
- What are Sky's highest-rated shows on each platform?
- Which platform offers the most content that both Tay and Landen would enjoy?
- Recommend shows on Disney+ that match Hanna's preferences
- Show me highly-rated content that's easily accessible (on major platforms)
```

**Timeline-Based Analysis:**
```
Using the timeline data in the file:
- What shows are getting new seasons soon that each person should be excited about?
- Which recently ended shows (2020+) might each person have missed?
- Find ongoing shows (no end date) that match each person's taste
- What's the best decade for each person's entertainment preferences?
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