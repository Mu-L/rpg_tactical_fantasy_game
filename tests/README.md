# Test Harness Guide

## Writing Tests
- Stick to the Arrange → Act → Assert pattern and assert on behaviors, not internal data.
- Test cases should be self explanitory and comments kept to a minimum. 
- Define commonly use variables at the class level for each testing module. 
- Reuse helpers in `tests.tools` and `tests.random_data_library` for brevity.

## Running Tests
- Full suite: `uv run pytest tests`.
- Single module: `uv run pytests tests/test_shop.py`.

## Warnings
- WARNING: Tests must be launched for development purposes only.
Tests may change your game configuration (as an example, your saves could be deleted !).
- WARNING: The game must be set to English before running tests. Other languages will cause test case failue. 
