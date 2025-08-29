# CallQualityAnalyzer
This CallQualityAnalyzer, analyzes the call between a customer and a sales representative using python and also evaluates the following:
1. Talk-time ratio (what % each person spoke)
2. Number of questions asked
3. Longest monologue duration
4. Call sentiment (positive/negative/neutral)
5. One actionable insight
I started by converting the video's audio into a WAV file with 16kHz mono format and then I performed speaker diarization on it using a combination of voice activity detection(VAD) and clustering to identify segments spoken by each person. Using those segments, i calculated metrics like talk-time percentage per speaker, longest monologue, number of short questions per speaker, call sentiment, and generated a simple actionable insight. I also roughly assign roles based on who talks more. Normally, the notebook could fetch YouTube transcripts directly, but because of YouTube restrictions downloading the video through code couldn't happen, so I had to download the video locally on my laptop and then upload it to my colab notebook.
