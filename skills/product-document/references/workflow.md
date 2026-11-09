# Product document workflow

This diagram is the canonical sequence. Terra owns evidence, CAD rendering, production layout, and verification. Imagegen owns visual concept generation and raster edits. Selection may already be supplied by the user; a request to finish a particular concept is sufficient.

```mermaid
flowchart TD
    A[Terra: establish authoritative content, format and references] --> B[Terra: inspect actual CAD and render multiple product views]
    B --> C[Imagegen: create complete themed concepts using CAD views, content and design references]
    C --> D[Terra: present concepts and record selection]
    D --> E[Imagegen: edit selected concept to retain background only]
    E --> F[Imagegen: separately extract decorative illustrations from selected original with transparency]
    F --> G[Terra: match each depicted product pose, camera and framing in actual CAD]
    G --> H[Terra: render with appropriate real materials, texture and lighting]
    H --> I[Terra: replace every generated product depiction with its matched render]
    I --> J[Terra: rebuild authoritative text, layout and simple geometry as editable vectors]
    J --> K[Terra: inspect every page, product and copy; export and deliver]
    classDef terra fill:#cfe6ff,stroke:#2463a0,color:#10243a;
    classDef imagegen fill:#f5d6ef,stroke:#9b387f,color:#3b1732;
    class A,B,D,G,H,I,J,K terra;
    class C,E,F imagegen;
```

Backgrounds, paintings and textures normally remain raster. Simple geometry is editable vector artwork. Suitable illustrations or backgrounds may be vectorized on request where fidelity permits. Preserve the original concept, background, transparent decorations, CAD renders, editable source, and export as separate assets. Track revision, selection, prompts and provenance; do not label generated hardware as a CAD render.
