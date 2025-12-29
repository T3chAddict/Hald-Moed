# Hald Moed Theatre Projects

This repository tracks and documents all Hald Moed theatre productions, including show files, audio assets, technical notes, and workflows. This documentation serves as a reference for how we organize and execute our productions.

## 📋 Table of Contents

- [Overview](#-overview)
- [Project Structure](#-project-structure)
- [Current Productions](#-current-productions)
- [Tools & Software](#%EF%B8%8F-tools--software)
- [Workflow Documentation](#-workflow-documentation)
- [File Organization](#-file-organization)
- [Best Practices](#-best-practices)
- [Resources](#-resources)

## 🎭 Overview

This repository serves as the central hub for all Hald Moed theatre production files and documentation. Each production gets its own directory containing:

- **Show files**: QLC+ workspaces (`.qxw` files) for sound and lighting control
- **Audio assets**: Sound effects, music, and voice recordings
- **Technical notes**: Production-specific notes and cues
- **Documentation**: How we set up and run each show

## 📁 Project Structure

```
Hald-Moed/
├── */                     # Production slug name
│   ├── *.qxw              # QLC+ workspace files
│   ├── geluiden/          # Sound effects library
│   ├── nijslezzer/        # News reader audio files
│   └── opening-nummer-*.wav  # Opening number variations
├── README.md              # This file
├── LICENSE                # Copyright license
└── .gitignore             # Git ignore rules
```

### Directory Conventions

- **Production directories**: Named after the production (e.g., `ien_dei_frede/`)
- **Audio subdirectories**: 
  - `geluiden/` - Sound effects and ambient audio
  - `nijslezzer/` - Voice recordings (news reader segments)
- **Show files**: QLC+ workspace files (`.qxw`) - main file and backups

## 🎬 Current Productions

### Ien Dei Frede (2026)

**Audio Assets**:
- Sound effects: doorbell, gunshots, church bells, thunder, falling tree, TV channel switching
- News reader segments: 12 numbered audio files (various formats: `.wav`, `.m4a`, `.aup3`)
- Opening number: Multiple versions (v1, v2) for comparison

## 🛠️ Tools & Software

### QLC+

**Purpose**: Lighting control and fixture management

**File Format**: `.qxw` (QLC+ workspace files)

**Best Practices**:
- Always keep a backup copy of the workspace
- Test all cues before show day
- Document cue numbers and timing in production notes

**Web Interface**: Can be started for remote control
- Reference: [QLC+ Forum - Web Interface on Mac](https://www.qlcplus.org/forum/viewtopic.php?t=17717)

**Integration**: Works alongside QLC+ for synchronized lighting cues

### Audacity

**Purpose**: ???

**Formats Used**:
- `.wav` - Primary format for sound effects and voice recordings
- `.m4a` - Compressed format for some news reader segments
- `.aup3` - Audacity project files (source files, not used in show)

**Naming Conventions**:
- Sound effects: Descriptive names (e.g., `deurbel-v2.wav`, `biem-1-keer-v1.wav`)
- Voice recordings: Sequential numbering (e.g., `nijslezer-01.wav`, `nijslezer-02.wav`)
- Variations: Version suffixes (e.g., `-v1`, `-v2`)

## 📝 Workflow Documentation

### Starting a New Production

1. **Create Production Directory**
   ```
   mkdir production_name/
   cd production_name/
   ```

2. **Set Up Audio Directories**
   ```
   mkdir geluiden/
   mkdir nijslezzer/  # or other voice/character directories as needed
   ```

3. **Create QLC+ Workspace**
   - Open QLC+
   - Create new workspace
   - Save as `YYYY_Production_Name.qxw`
   - Advised: Create backup copy immediately

4. **Organize Audio Assets**
   - Collect all sound effects in `geluiden/`
   - Organize voice recordings by character/segment
   - Use consistent naming conventions

5. **Document in Production Notes**
   - Create `notities.txt` for production-specific notes
   - Document cue lists, timing, special requirements

### Pre-Show Checklist

- [ ] All audio files tested and working
- [ ] All cues numbered and documented
- [ ] Lighting cues synchronized with sound
- [ ] Special effects (strobe, thunder) tested
- [ ] Opening number version selected
- [ ] News reader segments in correct order
- [ ] Backup equipment ready

### During rehearsals

- Keep notes updated with:
  - Cue timing adjustments
  - Technical issues encountered
  - Changes made during rehearsals
  - Notes for next performance

### Post-Show

- Archive final workspace version
- Document any last-minute changes
- Note what worked well and what needs improvement
- Update this README with lessons learned

## 📂 File Organization

### Audio File Naming

**Sound Effects**:
- Format: `descriptive-name-v#.wav`
- Examples: `deurbel-v2.wav`, `biem-1-keer-v1.wav`
- Version numbers for A/B testing different takes

**Voice Recordings**:
- Format: `character-##.wav` or `segment-##.wav`
- Examples: `nijslezer-01.wav`, `nijslezer-02.wav`
- Sequential numbering for ordered segments

**Music/Opening Numbers**:
- Format: `description-v#.wav`
- Examples: `opening-nummer-v1.wav`, `opening-nummer-v2.wav`
- Keep multiple versions until final selection

### QLC+ Workspace Files

- **Main file**: `YYYY_Production_Name.qxw`
- **Backups**: `YYYY_Production_Name copy.qxw` (gitignored)
- **Version control**: Only commit the main workspace file

## ✅ Best Practices

### Version Control

- **Commit**: Main workspace files, final audio selections
- **Ignore**: Backup copies (`*copy.qxw`), personal notes (`notities.txt`)
- **Document**: Major changes in commit messages

### Audio Management

1. **Source Files**: Keep original recordings even after processing
2. **Format Consistency**: Convert all files to `.wav` for show use
3. **Naming**: Use clear, descriptive names that indicate purpose
4. **Organization**: Group related files in subdirectories
5. **Testing**: Test all audio files in QLC+ before show day

### QLC+ Workspace

1. **Backup Strategy**: Always maintain a backup copy
2. **Cue Organization**: Use clear cue names and grouping
3. **Documentation**: Add notes to complex cues
4. **Testing**: Run through entire show file before performance
5. **Version Control**: Only commit stable, tested versions

### Documentation

1. **Production Notes**: Use `notities.txt` for show-specific details
2. **README Updates**: Update this file with new workflows or tools
4. **Troubleshooting**: Note solutions to technical problems

## 🔗 Resources

### Sound Effects
- **Pixabay Sound Effects**: https://pixabay.com/sound-effects/search/
  - Free, high-quality sound effects library
  - Useful for finding ambient sounds, effects, and music

### QLC+ Lighting Control
- **QLC+ Forum - Web Interface**: https://www.qlcplus.org/forum/viewtopic.php?t=17717
  - Instructions for starting QLC+ web interface
  - Useful for remote lighting control

### QLC+ Resources
- Official QLC+ documentation and tutorials
- Community forums for troubleshooting

## 📌 Notes for Future Productions

### Common Workflows

- **Sound Effect Testing**: Import into QLC+, test volume levels, adjust timing
- **Voice Recording**: Record in consistent format, number sequentially, test playback
- **Lighting Sync**: Coordinate QLC+ cues with QLC+ sound cues
- **Version Control**: Always test before committing, keep backups separate

## 🤝 Contributing

When working on productions:

1. Create a branch for major changes
2. Test all changes before committing
3. Update documentation when adding new workflows
4. Keep production notes in `notities.txt` (not committed)
5. Commit stable, tested versions only

## 📄 License

See [LICENSE](LICENSE) file for details.

---

For questions or updates to this documentation, please update this README or create an issue.

