# Quick Reference

## Files in This Repository

| File | Purpose | Use Case |
|------|---------|----------|
| `entertainment_ratings.csv` | Main data file in CSV format | Upload to ChatGPT, easy to edit |
| `entertainment_ratings.xlsx` | Formatted Excel version | Better visual experience |
| `README.md` | Complete documentation | Learn about the system |
| `CHATGPT_GUIDE.md` | ChatGPT integration details | How to use with AI |
| `SAMPLE_PROMPTS.md` | Example prompts | Copy/paste prompts |
| `create_xlsx.py` | Conversion script | Regenerate XLSX from CSV |

## Quick Start (3 Steps)

1. **Open ChatGPT**: Go to https://chat.openai.com
2. **Upload**: Click 📎 and select `entertainment_ratings.csv`
3. **Ask**: Try this prompt:
   ```
   Based on Sky's favorites (TRUE) and high ratings, recommend 5 new items to try
   ```

## Data Schema

```
Type, Title, Genre, Sky_Rating, Tay_Rating, Sky_Favorite, Tay_Favorite, Notes
```

- **Type**: Movie | TV Show | Music Artist
- **Ratings**: 0-10 scale
- **Favorites**: TRUE | FALSE (carries extra weight)

## Sample Entry

```csv
Movie,Inception,Sci-Fi,9.0,8.5,TRUE,FALSE,Mind-bending thriller
```

## Most Common Tasks

### Add New Entry (CSV)
Open `entertainment_ratings.csv` and add a new line:
```csv
Movie,New Movie,Action,8.5,9.0,FALSE,TRUE,Great action scenes
```

### Regenerate XLSX
```bash
python3 create_xlsx.py
```

### Get Recommendations
Upload to ChatGPT and ask:
- "Recommend for Sky based on favorites"
- "What should Tay watch next?"
- "Find something both would enjoy"

## File Statistics

- **Total Entries**: 30 (10 movies, 10 TV shows, 10 music artists)
- **Sky Favorites**: 11 items
- **Tay Favorites**: 15 items
- **Shared Favorites**: 4 items (both marked TRUE)

## Editing Tips

✅ **DO:**
- Use consistent formatting (CSV structure)
- Rate on 0-10 scale
- Mark favorites strategically (they carry extra weight)
- Add helpful notes
- Keep entries organized by Type

❌ **DON'T:**
- Mix up column order
- Use commas in titles (breaks CSV) - use semicolons or dashes instead
- Forget to regenerate XLSX after CSV changes
- Leave required fields empty

## ChatGPT Prompt Templates

**Basic:**
```
Based on [Sky/Tay]'s ratings and favorites, recommend [number] [movies/TV shows/music] 
they might enjoy. Explain your reasoning.
```

**Advanced:**
```
Analyze both Sky and Tay's preferences. Find patterns in their favorites, 
then recommend items they could enjoy together. Prioritize favorites (TRUE).
```

**Discovery:**
```
Based on this data, suggest new content outside their usual preferences 
but still likely to be enjoyed. Explain the connections to their current favorites.
```

## Need Help?

1. See `README.md` for full documentation
2. Check `CHATGPT_GUIDE.md` for detailed ChatGPT instructions
3. Browse `SAMPLE_PROMPTS.md` for ready-to-use prompts
4. Run `python3 create_xlsx.py` to regenerate formatted Excel file

## Next Steps

1. ✏️ Replace sample data with your actual preferences
2. 📤 Upload to ChatGPT for personalized recommendations
3. 🔄 Update regularly as you watch/listen to new content
4. 🎯 Refine your prompts based on recommendation quality
