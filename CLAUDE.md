# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Context

This is Chapter 8 of a VibeCoding study project (2604 series). Shopping list web app backed by Supabase.

## Architecture

- `shopping-list.html` — single-file app (HTML + CSS + JS). No build step needed; open directly in a browser.
- Data is stored in Supabase table `Shopping_items` (columns: `id uuid PK`, `text text`, `checked boolean`, `created_at timestamptz`).
- Supabase JS client loaded via CDN (`@supabase/supabase-js@2`).
- Row Level Security is enabled with public CRUD policies (anon role allowed).

## Running

Open `shopping-list.html` in any browser. No server required.
