# TextScape

**A Confabulation-Inspired Text Knowledge Explorer**

TextScape transforms your written content into a navigable knowledge graph, leveraging principles from confabulation theory to uncover hidden connections and patterns.

---

## Features

- **Semantic Chunking**: Automatically breaks text into discrete "knowledge units" (paragraphs or sections).
- **Confabulation-Inspired Associations**: Builds weighted links based on co-occurrence strength and semantic similarity.
- **Activation Spreading**: Select a node to simulate neural activation and reveal related concepts.
- **Interactive Visualization**: Explore your corpus via a force-directed graph (D3.js) with zoom, pan, and drag.
- **Search & Highlight**: Find nodes matching queries and highlight them in the graph.

---

## Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Brave, Edge)
- Git & GitHub account

### Installation & Setup

1. **Clone this repo**
   ```fish
   git clone https://github.com/Innomen/textscape.git
   cd textscape
   ```

2. **Open in browser**
   - Double-click `text_scape.html` or serve locally:
     ```fish
     # with Python 3
     python -m http.server 8000
     open http://localhost:8000/text_scape.html
     ```

### Usage

- **Upload** `.txt` or `.md` files via the sidebar.
- **Add** text directly in the text area.
- **Click** a node to view full content and related concepts.
- **Search** to highlight matching nodes.
- **Drag/Zoom** to navigate large graphs.

---

## Architecture

- **Frontend**: HTML + D3.js for visualization, plain JavaScript modules
- **Text Processing**: Simple tokenizer & paragraph splitter
- **Association Engine**: Basic TF-style embeddings & cosine similarity
- **Activation Model**: Spreading activation based on link strength

For full details, see comments in `text_scape.html`.

---

## Roadmap

- Integrate advanced NLP (spaCy, embeddings)
- Support additional formats (HTML, PDF)
- Server-side processing for large corpora
- Persistent storage (MongoDB, Graph DB)

---

## Contributing

1. Fork the repo
2. Create a feature branch
3. Submit a pull request

---

## License

MIT License © Your Name

