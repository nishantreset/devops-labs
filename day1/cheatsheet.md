# Day 1 – Linux Basics Cheat Sheet

## 1️⃣ Navigation & Listing
pwd                  # Show current working directory
ls                   # List files/folders
ls -la               # Detailed list incl. hidden files
cd ..                # Go up one level
cd -                 # Jump to previous directory

## 2️⃣ Create & Edit Files/Folders
mkdir name           # Create folder
mkdir -p parent/child # Create nested folders
touch file           # Create empty file
echo "text" > file   # Write (overwrite) file
echo "text" >> file  # Append to file

## 3️⃣ Copy, Move, Rename
cp src dest          # Copy file
cp -r src dest       # Copy folder
mv old new           # Rename/move file or folder

## 4️⃣ Delete (Safe vs Dangerous)
rm file              # Delete file
rm -r folder         # Delete folder recursively
rm -ri folder        # Safe delete w/ prompt
# Avoid: rm -rf *    # DANGEROUS

## 5️⃣ View File Contents
cat file             # Show file content
head -n 5 file       # First 5 lines
tail -n 5 file       # Last 5 lines
less file            # Scroll view (q to quit)
wc -l file           # Count lines

## 6️⃣ Search & Find
find path -type f -name "*.ext"   # Find files by extension
grep -Rin "text" path             # Search text in files

## 7️⃣ Redirection & Pipes
cmd > file           # Send output to file (overwrite)
cmd >> file          # Append output to file
cmd1 | cmd2          # Pipe output of cmd1 into cmd2

## 8️⃣ Quick HTTP Server
python3 -m http.server 8080       # Serve files on port 8080

## 9️⃣ Safety Practices
pwd before rm -r    # Check location before deleting
Use rm -ri for safety
Avoid sudo unless required
