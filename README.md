# videomaker

# Video Merger Application

A Python-based application for merging video files, allowing users to select directories and customize merge settings. The application uses MoviePy and PyQt5 to provide a graphical user interface.

## Features

- **Dynamic Path Selection:** Users can select video directories and output directories through the GUI.
- **Customizable Merge Settings:** Adjust the number of files to merge at once and the merge interval.
- **Multiple Processing Methods:** Supports asyncio, threading, multiprocessing, joblib, and dask.
- **Audio Inclusion/Exclusion:** Option to include or exclude audio in the merged videos.
- **Parallel Processing:** Videos are processed in parallel to speed up the merging process.
- **Error Handling:** Robust error handling and logging.

## Requirements

- Python 3.6+
- MoviePy
- PyQt5
- asyncio
- concurrent.futures
- multiprocessing
- joblib
- dask
- dask.distributed

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/video-merger.git
    cd video-merger
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Run the application:
    ```bash
    python video_merger.py
    ```

2. Use the GUI to:
    - Select the video directory containing the videos to be merged.
    - Select the output directory where the merged videos will be saved.
    - Load the video list text file.
    - Set the number of files to merge at once.
    - Set the merge interval.
    - Choose whether to include audio or not.
    - Start the merging process.

## GUI Overview

- **Video Dizini Seç:** Select the directory containing the videos to be merged.
- **Çıktı Dizini Seç:** Select the directory where the merged videos will be saved.
- **Başlat:** Start the merging process.
- **Durdur:** Stop the merging process.
- **Duraklat:** Pause the merging process.
- **Devam Et:** Resume the merging process.
- **Çekirdek Sayısı:** Set the number of parallel workers for processing.
- **Ses Seçenekleri:** Choose whether to include audio in the merged videos.
- **Birleştirme Aralığı:** Set the interval for merging.
- **Kaçarlı Birleştirilecek Dosya Sayısı:** Set the number of files to merge at once.

## Customization

You can modify the default settings in the `VideoMerger` class:

- `self.video_dir`: Default video directory.
- `self.output_dir`: Default output directory.
- `self.max_workers`: Number of parallel workers.
- `self.include_audio`: Include audio in merged videos.
- `self.merge_interval`: Interval for merging.
- `self.group_size`: Number of files to merge at once.

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [MoviePy](https://zulko.github.io/moviepy/)
- [PyQt5](https://riverbankcomputing.com/software/pyqt/intro)

