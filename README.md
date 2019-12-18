## Summary of the modle
1. Use heart-sound audio data to identify heart disease, which has real world implication
2. Used transfer-learning of VGG19, with all weights locked
3. Applied onset method to crop the spectrogram data from the first peak
4. Tried normalization methods, which did not work very well compared to raw numbers. So ended up with raw spectrogram numbers
5. Also tried CNN plus LSTM, which performed poorlly.
6. Working environment is a VM on remote server. 8G RAM, no GPU. "Memory error" is a real concern, which is the reason to train 10 epoches a time and only harvest 6 second data with 50 dimensions
