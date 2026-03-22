<h1 align="center">Hardik Jindal</h1>
<p align="center">
  Software Engineer focused on <b>Applied ML Systems</b>, <b>Security Engineering</b>, and <b>Production APIs</b>.
</p>

<p align="center">
  <a href="https://github.com/06hardik"><img src="https://img.shields.io/badge/GitHub-06hardik-181717?style=for-the-badge&logo=github" alt="GitHub"></a>
  <a href="https://www.linkedin.com/in/hardik-jindal-a5b8a8325/"><img src="https://img.shields.io/badge/LinkedIn-Hardik%20Jindal-0A66C2?style=for-the-badge&logo=linkedin" alt="LinkedIn"></a>
  <a href="mailto:hardikjindal2020@gmail.com"><img src="https://img.shields.io/badge/Email-hardikjindal2020@gmail.com-informational?style=for-the-badge&logo=gmail" alt="Email"></a>
  <img src="https://komarev.com/ghpvc/?username=06hardik&style=for-the-badge&label=PROFILE+VIEWS" alt="Profile views">
</p>

## Engineering Profile
I build end-to-end systems where model logic, API design, and runtime behavior all matter.
My recent work spans citation-quality validation pipelines, low-latency event classification, and full-stack TypeScript applications.

- Primary languages: `Python`, `TypeScript`, `JavaScript`
- Core strengths: API contracts, ML inference pipelines, system design under constraints, debugging production behavior
- Work style: reproducible builds, explicit interfaces, measurable failure modes, maintainable code paths

## Core Technical Capabilities
| Area | Practical Scope |
|---|---|
| Backend/API Engineering | FastAPI service design, request/response contracts, status semantics (`ok/partial/failed`), integration-ready endpoints |
| ML Systems | Training + evaluation pipelines, ONNX export/inference, feature/token pipelines, CPU-optimized runtime decisions |
| Security-Oriented Engineering | Runtime event monitoring, Frida hooks, suspicious event classification, configurable filtering + audit logs |
| Full-Stack Development | React + Vite + TypeScript frontends, Node/JS tooling, modular backend/frontend repository layouts |
| Delivery & Operations | Dockerized services, dependency isolation, CI workflows, reproducible local setup and deployment entry points |

## Flagship Systems
### 1) [Research-Paper-Model](https://github.com/06hardik/Research-Paper-Model)
Production-style API for reference section quality analysis.

- Exposes hosted HTTP endpoints (`/health`, `/analyze`) with a documented integration contract.
- Pipeline evaluates citation style detection (IEEE/APA/MLA/Harvard/Vancouver), ordering, DOI presence, journal casing, completeness, and style conformity.
- Supports operational modes like `dry_run` and `deep_doi`, with explicit latency/accuracy trade-offs.
- Returns structured parser summaries and issue-level diagnostics designed for direct UI consumption.
- Includes Dockerized runtime and clear client integration paths for Python and JavaScript consumers.

### 2) [CYBER-SECURE-SCADA](https://github.com/06hardik/CYBER-SECURE-SCADA)
Real-time SCADA file-access defense prototype combining runtime hooks and ML inference.

- Integrates Frida-based instrumentation with a Python orchestrator for event capture.
- Uses an ONNX classifier for fast event verdicting (BENIGN/MALICIOUS) with confidence output.
- Maintains a full training pipeline (`data_gen`, tokenization, train, evaluate) and model export path.
- Implements a compact micro-transformer architecture (2 layers, 4 heads, ~120K params) targeting low-latency CPU inference.
- Includes simulator-driven validation and executable packaging path for operational testing.

### 3) [VividReel](https://github.com/06hardik/VividReel) / [Vivid_Reel](https://github.com/06hardik/Vivid_Reel)
End-to-end AI video editing pipeline built for EventVision (Innovision NSUT), where our team secured 2nd position by optimizing for robustness under real footage variability.

- Built with collaborators MOHAK BANSAL and Jayant Chauhan, with clear subsystem ownership and integration-driven delivery.
- Core architecture is cascade-based (not single-model): scene segmentation (PySceneDetect) -> frame sampling (16 key frames per micro-scene) -> primary transformer inference (fine-tuned VideoMAE) -> confidence gating.
- Low-confidence outputs are routed to fallback layers to improve reliability on noisy or low-quality inputs.
- Model cascade combines: VideoMAE (primary intelligence), Random Forest fallback, and a heuristic safety layer for edge-case handling.
- Random Forest uses an 11-feature engineered vector including focus (Laplacian variance), motion (frame differencing), face count (Haar Cascade), and emotion probabilities (DeepFace).
- Scenes are confidence-ranked and selected to fit a 5-10 minute target runtime.
- Final assembly is generated with MoviePy using mood-based pacing, transitions, dynamic slow motion, and context-aware background music.
- Data and scale used in development: 1300+ videos, ~7000 sub-clips, ~112k frames; datasets included Kinetics-400, HMDB51, and competition data.
- Stack: Python, FastAPI, VideoMAE, OpenCV, DeepFace, scikit-learn, MoviePy.
- Key engineering takeaway: reliability improved significantly by combining transformers with classical ML and domain heuristics instead of relying on a single model.

### 4) [Hack4Delhi-Sampark](https://github.com/06hardik/Hack4Delhi-Sampark)
Multi-module hackathon system with frontend, backend, and CV service separation.

- Repository structure includes distinct `frontend`, `backend`, and `cv_service` modules.
- Frontend stack uses Vite + React + TypeScript + Tailwind/shadcn patterns.
- Includes ML/CV assets in the project layout, enabling experimentation with vision-assisted workflows.

### 5) Additional Product Builds
- [DBT-Sahayak](https://github.com/06hardik/DBT-Sahayak): TypeScript-heavy project with separated `PUBLIC` and `SERVER` modules.
- [tournafy](https://github.com/06hardik/tournafy): collaborative tournament platform concept with frontend + backend structure.

## Technology Stack
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI">
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB" alt="React">
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite">
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/ONNX_Runtime-005CED?style=flat-square&logo=onnx&logoColor=white" alt="ONNX Runtime">
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" alt="PyTorch">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git">
</p>

## Engineering Standards
- Prefer explicit interface contracts and typed payloads over implicit assumptions.
- Build for observability: structured output, failure categorization, and debuggable runtime states.
- Separate training/inference/runtime concerns for ML-backed systems.
- Keep integration friction low with copy-paste client examples and predictable endpoint behavior.

## GitHub Analytics
<p>
  <img src="https://github-readme-stats.vercel.app/api?username=06hardik&show_icons=true&hide_title=true&rank_icon=github" alt="GitHub stats">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=06hardik&layout=compact" alt="Top languages">
</p>

## Open To
- Software Engineering Internships
- Applied ML / AI Engineering roles
- Security-focused engineering projects
- Open-source collaborations with clear technical ownership

## Contact
- Email: `hardikjindal2020@gmail.com`
- GitHub: [github.com/06hardik](https://github.com/06hardik)
- LinkedIn: [linkedin.com/in/hardik-jindal-a5b8a8325](https://www.linkedin.com/in/hardik-jindal-a5b8a8325/)

---
If you are hiring for strong execution in APIs, ML integration, and security-oriented systems, I would be glad to connect on [LinkedIn](https://www.linkedin.com/in/hardik-jindal-a5b8a8325/) or by email.
