### Before running docker
Directory structure before running docker

```
.
├── Readme.md
└── test_scene.py

1 directory, 2 files
```

### Docker command
```bash
docker run --rm -it  --user="$(id -u):$(id -g)" -v "$(pwd)":/manim manimcommunity/manim manim test_scene.py SquareToCircle -qm
```

### Directory after running docker

```
.
├── Readme.md
├── __pycache__
│   └── test_scene.cpython-38.pyc
├── media
│   ├── images
│   │   └── test_scene
│   └── videos
│       └── test_scene
│           └── 720p30
│               ├── SquareToCircle.mp4
│               └── partial_movie_files
│                   └── SquareToCircle
│                       ├── 207390714_1190651494_247722528.mp4
│                       ├── 207390714_1912732880_247722528.mp4
│                       ├── 274514146_549496807_223132457.mp4
│                       └── partial_movie_file_list.txt
└── test_scene.py
```
