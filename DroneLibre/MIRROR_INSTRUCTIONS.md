# Mirror Instructions

The cleanest way to archive the O-GS repository is a true git mirror. This preserves commit history, tags, branches, and file structure.

## Recommended Local Mirror

```bash
git clone --mirror https://github.com/o-gs/dji-hardware-schematics.git
cd dji-hardware-schematics.git
```

Then push it into a repository you control, ideally a dedicated repo such as:

```text
dronemaker-alt/dji-hardware-schematics-mirror
```

If the destination repo already exists and is empty:

```bash
git remote set-url origin https://github.com/dronemaker-alt/dji-hardware-schematics-mirror.git
git push --mirror
```

## Alternative: Subtree / Vendor Copy

If keeping the material inside Ragnarok instead of a separate mirror:

```bash
git clone https://github.com/dronemaker-alt/Ragnarok.git
cd Ragnarok
mkdir -p DroneLibre/Upstream_Archive
cd DroneLibre/Upstream_Archive
git clone https://github.com/o-gs/dji-hardware-schematics.git o-gs_dji_hardware_schematics
cd ../../..
git add DroneLibre/Upstream_Archive/o-gs_dji_hardware_schematics
git commit -m "Archive O-GS DJI hardware schematics"
git push
```

This does not preserve the upstream repository history inside Ragnarok unless handled as a subtree or submodule.

## Submodule Option

A submodule keeps a pointer to upstream but does not fully preserve an independent copy if upstream disappears.

```bash
git submodule add https://github.com/o-gs/dji-hardware-schematics.git DroneLibre/Upstream_Archive/o-gs_dji_hardware_schematics
git commit -m "Add O-GS DJI hardware schematics submodule"
git push
```

Use this only as a convenience pointer, not as the only archive.

## Archive Preference

Best archival strategy:

1. Create a dedicated mirror repo.
2. Keep curated notes and depot workflow inside Ragnarok.
3. Copy only high-value reference files into Ragnarok when directly used by Drone Libre.
4. Keep source attribution in `SOURCE_LOG.md`.

## Suggested Dedicated Repositories

```text
dronemaker-alt/dji-hardware-schematics-mirror
dronemaker-alt/drone-libre-depot
dronemaker-alt/mini-2-repair-notes
```

Ragnarok can remain the master project hub, while the mirror repo preserves upstream history.
