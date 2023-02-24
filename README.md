# Cache requirements.txt

Version: 1.0.0

Loads a venv from a requirements.txt, with a cache wrapper

## Usage

```yaml

# It is better practice to use the SHA hash of this tag rather than the tag itself.
- uses: ajparsons/cache-requirements-txt@v1
  id: example-step 
  with:
    requirements_path: '' 
    cache_key: 'cache-key'  # default
    venv_path: '/tmp/venv_cache/'  # default
    python_version: '3.10'  # default

```

## Inputs

### requirements_path

path to requirements.txt

### cache_key

short-key-for-action

Default: cache-key

### venv_path

Venv path for action

Default: /tmp/venv_cache/

### python_version

python_version

Default: 3.10

## Outputs

### cache-hit

Was the cache used

