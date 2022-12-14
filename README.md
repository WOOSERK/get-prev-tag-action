# get-prev-tag-action

you can get previous tag with this action.

## Usage

```yaml
jobs:
  your-job:
    steps:
      - name: Checkout
        uses: actions/checkout@v3
        with:
          fetch-depth: 0 # must have item

      - name: Get Prev Tag
        id: prev-tag-finder
        uses: WOOSERK/get-prev-tag-action@v0.1.1

      - name: Echo your prev tag
        run: echo ${{ steps.prev-tag-finder.outputs.prev-tag }}
```

## ETC

- 22.12.15 v0.1.0 release
- 22.12.15 v0.1.1 release
