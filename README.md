# AzbarkonData

Per-poet SQLite database files for the Azbarkon app.

Each `poet_<id>.s3db` contains all poems and search index (FTS4) of a single
poet from Ganjoor. Files are served through GitHub Releases:

```
https://github.com/fziraki/AzbarkonData/releases/latest/download/poet_<id>.s3db
```

- `manifest.json` — metadata for all 249 poets (id, name, slug, file, size, poem/verse counts).
- Default database with the 9 most popular poets is bundled inside the app itself.

## Rebuild

Source database is Ganjoor's public `ganjoor.s3db`. The builder script lives in
the app repo at `tools/poet_db_builder.py`.

## License

Data © Ganjoor (https://ganjoor.net), used per their public dataset terms.
