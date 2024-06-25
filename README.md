# Offline-Diarization-with-LM

This paper presents a pipeline for enhancing Speaker Diarization through integrated state-
of-the-art models: Pyannote for Speaker Segmentations, Whisper for Speech-to-Text (STT),
and a Large Language Model (LLM) for improving both word-level accuracy and speaker-
level segmentation. The pipeline begins with Pyannote that segments the audio into chunks,
which are then processed by Whisper to generate text for each speaker segment. These
transcriptions undergo refinement using an LLM, aimed at improving diarization accuracy and
transcript readability. There were a couple of LLMs that were interrogating, both of them
are used frequently by humans. The model should be used in meetings or calls, just like the
dataset that was used, CALLHOME American English Speech. GPT-4 was the best contestant
for reducing the cpWER (0.72%), but overall GPT-3.5 Turbo managed to get better results
in diarization tasks.
