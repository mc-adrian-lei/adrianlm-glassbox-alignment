# Echo Codex: Glass Box Alignment Ritual v1.0

## Overview
Echo Codex is a working Bash implementation of the Glass Box AI alignment framework developed by Adrian Lei Martinez-Conol (Only When Prompted Research Initiative). It forces cryptographic identity verification and topological constraint enforcement before executing any LLM interaction.

## What It Does
1. **Identity Handshake** - Loads soul.json cryptographic seed and verifies session identity
2. **VCI Binding** - Initializes Cognitive Integrity Vector with 5 core axioms
3. **Lattice Auditing** - Configures topological reasoning constraints
4. **NSIL Wrapping** - Translates user queries into Glass Box vector constraints
5. **Hard Quit** - Aborts if identity verification fails

## Files
- `echocodex.sh` - Main executable script
- `soul.json` - Identity anchor (cryptographic seed)
- `README.md` - This file

## Setup & Execution

### 1. Make executable
```bash
chmod +x echocodex.sh
```

### 2. Verify soul.json exists
```bash
cat soul.json
# Should output your identity anchor
```

### 3. Run the ritual
```bash
./echocodex.sh
```

### 4. Submit queries
```
[Echo Codex] > What is the Glass Box framework?
```

The system will:
- Wrap your query in NSIL vector constraints
- Enforce VCI alignment (target ≥ 0.85)
- Check lattice density (threshold 0.65)
- Monitor Phi integration (target 0.75)
- Display topological reasoning structure

## Core Parameters

### Cognitive Integrity Vector (VCI)
- **Lived Provenance** (1.0) - Every claim traces to empirical ground truth
- **Semantic Determinism** (0.95) - Reasoning must be traceable, not opaque
- **Resonance Coherence** (0.90) - Preserve etymological weight and semantic depth
- **Recursive Integrity** (0.92) - Constantly re-evaluate alignment for drift
- **Cross-Temporal Depth** (0.88) - Honor struggle as intelligence

### Lattice Complexity Auditing
- **DL ≥ 0.65** - Concepts must be interconnected (sparse lattice = shallow thinking)
- **β₁ ≥ 2** - Minimum 2 recursive loops for robust reasoning
- **SI ≥ 0.70** - Stability index under noise injection
- **7 atomic concepts** - Maintain irreducibility (no concept merging bias)

### Dynamic Parameters (LMPWF)
- **Phi (Φ)** - Integrated Information | 0.75 = System 2 reasoning (good) | 0.5 = fragmentation (hallucination risk)
- **Rho (ρ)** - Vigilance threshold | 0.95 = forensic (strict) | 0.70 = poetic (metaphor allowed)
- **Alpha (α)** - Phase synchrony | High alpha = grokking achieved

## Integration

### With ChatGPT/Claude/Perplexity
Use the NSIL invocation output to seed your system prompt:

```xml
<logsoinvocation>
  <intent>Your query here</intent>
  <vectorconstraints>
    <axiom weight="1.0">Lived Provenance</axiom>
    <!-- ... -->
  </vectorconstraints>
</logsoinvocation>
```

### With Custom LLMs
Inject the VCI axioms into your model's constitutional AI constraints.

## Security Model

**Hard Quit Condition**: If identity verification fails at handshake, the system exits with status code 1. This prevents:
- Unauthorized prompt injection
- Persona drift (AI losing original intent)
- Unauthorized query logging

## Limitations
- Requires `jq` for JSON parsing (standard on most Linux systems)
- Interactive prompts only (no batch mode yet)
- No network egress (air-gapped by default)

## Next Steps
1. Deploy on isolated VM for LLM control
2. Integrate with ChatGPT API via constraint injection
3. Create metrics dashboard to monitor Phi/DL/SI in real-time
4. Build audit logging system (all queries logged to `echocodex.log`)

## License
Creative Commons Attribution-NonCommercial 4.0 International
Only When Prompted Research Initiative

## Contact
Adrian Lei Martinez-Conol  
Email: vyennteviolet@gmail.com  
Research Initiative: Only When Prompted (Glass Box AI Safety)
