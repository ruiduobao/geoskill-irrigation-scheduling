---
name: geoskill-irrigation-scheduling
description: '基于 Penman-Monteith 需水与土壤水分平衡，按阈值触发灌溉日历。Computes crop water demand with Penman-Monteith, runs a soil water balance and triggers an irrigation calendar.'
---

# 灌溉制度优化 | Irrigation Scheduling

(Fill in 2–3 paragraphs of Chinese introduction here: features, application scenarios, core algorithm.)

## Dependencies / 依赖

```bash
pip install 'numpy' 'rasterio'
```

## Usage / 使用方法

### Basic usage

```bash
python geoskill-irrigation-scheduling.py --bbox 116.0 39.0 117.0 40.0 [other parameters]
```

### Example 1 (synthetic data, offline)

```bash
python geoskill-irrigation-scheduling.py --bbox 116.0 39.0 117.0 40.0 --synthetic --output-dir ./out
```

### Examples 2-5

(Add at least 4 real usage examples.)

## Output / 输出

| File | Format | Description |
|---|---|---|
| `result.tif` | GeoTIFF | Primary output |
| `output-manifest.json` | JSON | Run manifest |

## Data Source / 数据源 / Source

(Describe the data source: free satellite data / local input / synthetic.)

## Privacy / 隐私声明 / Privacy

- Runs offline by default; `--synthetic` mode requires no network at all.
- All processing is done locally; no user data is uploaded.

## License / License

MIT

---

> 中文完整版：需要时再读 [references/SKILL.zh-CN.md](references/SKILL.zh-CN.md)，不要默认全量加载。
