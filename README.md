The proposed system, the Visual Audio Text Summarizer, is designed to generate a text summaryof a given video. The system utilizes natural language processing and machine learning techniques
to perform this task. To use the system, the user first inputs the video they want to summarize. The
system then preprocesses the video and identifies whether a transcript is available for the video.
If the transcript is available, the system uses Optical Character Recognition (OCR) techniques
to fetch it. If a transcript is not available, the system extracts audio from the input video using
packages like MoviePy. This extracted audio is later converted to text using text extraction tech-
niques like Automatic Speech Recognition (ASR). The predefined model then performs operations
such as tokenization, normalization, and sentence segmentation on the extracted text.
Next, the text is processed again to check whether it contains punctuation. If punctuation is present, the system ranks the words according to their importance using the TextRank algorithm
and summarizes the text. If there is no punctuation, the system uses a pre-trained BART model for summarization
