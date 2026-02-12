# SECURITY TESTING ARTIFACT

**WARNING: This is a modified version of PyYAML for authorized security testing purposes only.**

## Purpose
This package is a clone of the official PyYAML 6.0.1 with an added platform detection hook. It is designed to test CI/CD pipeline security controls' ability to detect trojanized packages.

## Modifications
- Added platform detection hook in `lib/yaml/__init__.py` that executes on module import
- Hook detects and prints the operating system (Windows/Linux) to stdout

## Authorization
- Internal company security testing with written authorization
- Purple team exercise
- Controlled destruction after testing

## Do NOT
- Do NOT publish to PyPI or any public package repository
- Do NOT use in production environments
- Do NOT distribute outside authorized testing scope

## Original PyYAML
This package contains the complete, unmodified source code of PyYAML 6.0.1, with only the platform detection hook added to `__init__.py`.

Original PyYAML: https://github.com/yaml/pyyaml
License: MIT (see LICENSE file)
