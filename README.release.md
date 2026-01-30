# README.release

## Instructions

1. Clone the latest aspell-lang repository:
   ```bash
   git clone https://https.git.savannah.gnu.org/git/aspell/aspell-lang.git
   ```

2. Create a wordlist without special characters like `-`, `.`, `:`, `()`.

3. Sort the wordlist:
   ```bash
   sort wordlist.txt wordlist-final.txt
   ```

4. Copy `wordlist.txt` to `gu.wl`:
   ```bash
   cp wordlist.txt gu.wl
   ```

5. Prezip-compress the wordlist:
   ```bash
   prezip -z -s gu.wl
   ```

6. Run the `proc` script to create:
   ```bash
   ./proc create
   ```

7. Run the configuration script:
   ```bash
   ./configure
   ```