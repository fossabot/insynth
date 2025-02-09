# insynth

---

[![Codacy Badge](https://app.codacy.com/project/badge/Grade/069d3759b9e24a468bd4f47c0c3fd02f)](https://www.codacy.com/gh/mlxyz/insynth/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mlxyz/insynth&amp;utm_campaign=Badge_Grade)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=mlxyz_insynth&metric=bugs)](https://sonarcloud.io/summary/new_code?id=mlxyz_insynth)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=mlxyz_insynth&metric=coverage)](https://sonarcloud.io/summary/new_code?id=mlxyz_insynth)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fmlxyz%2Finsynth.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fmlxyz%2Finsynth?ref=badge_shield)

# Testing Audio Perturbators
```python
from insynth.perturbators.audio import AudioShortNoisePerturbator
import librosa
from scipy.io.wavfile import write
perturbator = ...
signal, sr=librosa.load(file_name, sr=None)
result = perturbator.apply((signal, sr))
write("output.wav", sr, result)
```

## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fmlxyz%2Finsynth.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fmlxyz%2Finsynth?ref=badge_large)