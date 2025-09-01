# Task-06_Deep-Fake — Syracuse University Women’s Lacrosse (2023–2024)

**Author:** Apoorva Mahajan — amahaj05@syr.edu  

This project extends Task-05 (Descriptive Stats & LLM comparison) and uses the same verified data to create an AI-generated interview summarizing the 2024 season.

Focused on the 2023–2024 Syracuse University Women’s Lacrosse cumulative statistics, comparing them to the 2023 season and highlighting improvements, challenges, and player performances. Using this dataset, I generated a mock interview script and experimented with **text-to-speech (TTS) and video avatar tools** to simulate an AI “deep fake” sports interview. I was able to replicate an AI-generated video via Vrew.ai; however, not in a street interview style format due to the tool limitations.

---

## Workflow & Process

### Step 1: Data Sources (please get in contact with amahaj05@syr.edu for the datasets)
- 2023 SU Women’s Lacrosse Cumulative Statistics (Excel)
- Player Improvement CSV (tracking year-over-year point increases)
- Team Stats Comparison CSV (efficiency, turnovers, assists, shooting %)

These structured datasets formed the foundation for building my sports analysis narrative.

### Step 2: Narrative Creation
- Summarized key performance trends:
  - Increased shot attempts (~55/game)
  - Shooting percentage decline (~20.6%)
  - Turnovers rise (~26.6/game)
- Identified standout players:
  - Emma Tyrrell (92 pts)
  - Olivia Adamson (83 pts)
  - Payton Rowley (+36 improvement year-over-year)
- Drafted a Q&A style script (saved in `scripts/lacrosse_interview.md`).

### Step 3: Audio Generation (ElevenLabs)
- Imported the script into ElevenLabs TTS.
- Generated two voices (Interviewer + Analyst).
- Exported conversation as MP3 (saved in `media/audio/`).

### Step 4: Attempting Video Generation
- Goal: Create a deep fake interview video.
- Tools tested: CapCut, D-ID trial, HeyGen trial, Vrew.ai
- Challenges: Free versions restrict voices, avatars, export length, and quality.
- Workaround: Tried combining ElevenLabs MP3 with CapCut for subtitles, creating a sports-style audio interview with visuals.

### Step 5: Repository Documentation
Organized files for reproducibility:
```
/task_05_script_&_documentation (previous task python script and documentation pdf)
/task06_scripts - SU_Womens_lacrosse_interview_script.md
/media - SU_Womens_lacrosse_interview_final.mp3, SU_lacross_subtitles.srt, SU_Lacrosse_video.mp4
Task_06_Deep_Fake_SU_Lacrosse_Workflow_Log.pdf
README.md
```

## How to reproduce (step-by-step)

### A. Prepare the script (already provided)
1. Use `notebooks/Task_05_...ipynb` from Task 05 to confirm numbers (top scorers, improvements, team trends).
2. Copy `scripts/interview_script.md` — this is the exact text to feed into ElevenLabs TTS.

### B. Generate audio (ElevenLabs — free tier)
1. Sign up at https://elevenlabs.io and log in.
2. Open **Text-to-Speech / Studio**.
3. Pick a free voice from the voice library and preview it.
4. Paste one script paragraph at a time (short chunks), adjust pronunciation hints if required.
5. Click **Generate** and then **Download** the MP3.
6. Repeat for each script chunk and combine in your editor if needed.

### C. Assemble the video (CapCut or Shotcut or Hey Gen)
1. Create a new project; import background footage, player photos, and the generated MP3(s).
2. Place audio on the timeline, then add text overlays and stat cards per the shot list.
3. Import `medias/subtitles.srt` or paste subtitles manually.
4. Export as `medias/interview.mp4` (1080p recommended).
---

## Tools & Resources
- Data Analysis: Excel + CSVs  
- Scriptwriting: Manual (based on stats comparison)  
- Text-to-Speech: ElevenLabs  
- Video Attempts: CapCut, D-ID trial, HeyGen trial, Vrew.ai  
- Subtitles: Auto-generated in CapCut  

---

## Results
- 🎧 **Audio Interview**: `media/audio/interview_final.mp3`  
- 📝 **Transcript/Script**: `scripts/lacrosse_interview.md`  
- 📊 **Stats Source**: 2023–24 Lacrosse dataset (Excel & CSVs)  

While I was unable to produce a fully polished “deep fake” street interview video due to free-tool limitations, I successfully:
1. Converted structured stats → narrative script.  
2. Generated multi-voice audio simulating an interview.  
3. Created subtitles + structured repo for reproducibility.  

---

## Challenges & Reflections
- **Tool limitations**: Most free tools limited voices, avatars, or export time.  
- **Creative adjustment**: Delivered an audio-based sports interview with subtitles instead of a full deepfake video using Vrew.ai.  
- **Future steps**: Use HeyGen/D-ID paid versions for full talking-head avatars, RunwayML for video editing, and Premiere Pro for advanced editing.  

---

## Conclusion
This task showed how structured sports data can be transformed into a compelling sports media product using AI. Even without perfect deep fake tools, I demonstrated how to:  
- Summarize statistics into narratives  
- Apply AI voices to simulate interviews  
- Explore limitations and workarounds of free video-generation platforms

## Ethics & Notes
- All numbers in the media come from the Task-05 Python outputs (see Task 05 notebook).
- Media is labeled as AI-generated and used only for academic purposes.


## Contact
For dataset access or questions: amahaj05@syr.edu  
