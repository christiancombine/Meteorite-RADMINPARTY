Metourite Source with some improvements 
GO TO Front/src/lib/url.ts 
CHANGE MY RADMIN IP TO YOURS ENJOY!
backend is easy enough
front rarely needs shit tho i patched it
just get pnpm and enjoy


 useful for ur parties ok host it for ur friends idk 
[ DO NOT USE THIS FOR NOW ILL UPLOAD PATCHES SOON! ]

ultimate PATCH HERE changeds my ip to shit ok
Get-ChildItem -Recurse -Include *.ts,*.js,*.svelte | ForEach-Object {
    $content = Get-Content $_.FullName -Raw
    $content = $content -replace 'import\s*\{\s*26.186.176.105\s*\}\s*from\s*["'']\$env/static/public["''];?', ''
    $content = $content -replace 'http://\$\{26.186.176.105\}', 'http://yourradminip'
    Set-Content $_.FullName $content
}
