# Sample ChatGPT Prompts

This file contains example prompts you can use with the entertainment ratings file.

## Upload Instructions

1. Go to ChatGPT (https://chat.openai.com)
2. Click the paperclip icon to upload a file
3. Select `entertainment_ratings.csv` or `entertainment_ratings.xlsx`
4. Use any of the prompts below

---

## Basic Recommendation Prompts

### For Sky:
```
I've uploaded my entertainment ratings. Based on Sky's ratings and favorites (marked TRUE), 
please recommend:
- 3 movies to watch
- 2 TV shows to binge
- 2 music artists to explore

Prioritize items similar to those marked as favorites.
```

### For Tay:
```
Looking at Tay's preferences in the uploaded data, recommend 5 new items 
(movies, TV shows, or music) that match their taste. Explain why each 
recommendation fits based on their rating patterns and favorites.
```

---

## Advanced Analysis Prompts

### Compatibility Analysis:
```
Analyze the uploaded entertainment ratings and tell me:
1. What do Sky and Tay have in common in their taste?
2. Where do their preferences differ the most?
3. Recommend 3 items they could enjoy together (both would rate 8.5+)
```

### Genre Preferences:
```
Based on the uploaded ratings:
- What are Sky's top 3 genres across all categories?
- What are Tay's top 3 genres?
- For each person, suggest one item from an underexplored genre they might enjoy
```

### Deep Dive:
```
Act as a personalized recommendation engine. Using the uploaded data:

For Sky:
1. Identify the key characteristics of their favorites
2. Find patterns in their high-rated items
3. Recommend 5 NEW items (not in the list) with detailed reasoning

For Tay:
Do the same analysis and provide 5 recommendations

Consider genre, themes, style, and the favorite flags for extra weight.
```

---

## Specific Scenario Prompts

### Movie Night:
```
It's movie night! Based on both Sky and Tay's ratings, suggest:
- 3 movies they'd both enjoy (consider favorites and ratings 8+)
- For each, explain why both would like it
- Order them from most to least likely to satisfy both
```

### Discovery Mode:
```
Based on this data, what new content should each person try that's 
outside their comfort zone but still likely to be enjoyed?

For each suggestion, explain:
- Why it's a stretch (different from usual preferences)
- Why they'd still likely enjoy it (subtle connections to favorites)
```

### Quick Picks:
```
I need quick recommendations:
- One movie for Sky to watch tonight
- One TV show for Tay to start this weekend
- One music artist both should check out together

Keep it brief, 1-2 sentences per recommendation.
```

---

## Maintenance Prompts

### Rating Analysis:
```
Analyze the rating patterns in this data:
- Average ratings per person
- Rating distribution (how many 9+, 8-9, 7-8, etc.)
- Most agreed upon items (similar ratings)
- Most divisive items (biggest rating difference)
```

### Missing Genres:
```
Based on the uploaded ratings, which genres or types of entertainment 
are underrepresented? Suggest specific titles to add to diversify 
the collection while matching each person's preferences.
```

---

## Follow-Up Conversation Example

**Initial Upload:**
```
I've uploaded our entertainment ratings. Please analyze both Sky and 
Tay's preferences and give me an overview of their tastes.
```

**After AI Response:**
```
Great analysis! Now recommend 5 movies for a marathon that both would 
enjoy, starting with the most universally appealing.
```

**Refining:**
```
Those are good, but focus more on sci-fi and fantasy genres since I 
noticed both enjoy those. Any recommendations?
```

**Adding New Ratings:**
```
I've updated the file with 5 new entries. Based on these new ratings, 
do you see any new patterns? Should your recommendations change?
```

---

## Tips for Best Results

1. **Be specific**: Mention which person, how many recommendations, what type
2. **Reference favorites**: These carry extra weight in the algorithm
3. **Ask for reasoning**: Understanding "why" helps validate recommendations
4. **Iterate**: Refine based on initial recommendations
5. **Context matters**: Mention mood, occasion, or constraints

## What NOT to Do

❌ "Recommend something good"
   → Too vague, doesn't use the data effectively

❌ "What movies are in the file?"
   → AI can read it, but this doesn't leverage its recommendation capability

✅ "Based on Sky's sci-fi favorites rated 9+, recommend similar movies"
   → Specific, data-driven, actionable

✅ "Find items both Sky and Tay marked as favorites and explain what they have in common"
   → Analytical, uses the data structure effectively
