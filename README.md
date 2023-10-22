# laba1_bat
<<<<<<< HEAD
# laba1_sh
# laba1_sh
=======
@echo off
setlocal enabledelayedexpansion

set /p input=Vvedite put' k papke:
set "fas=%input%"

if exist "%fas%" (
  echo dannaja papka jest
) else (
  echo dannoj papki net
)
pushd "%fas%"

set i=1
for %%f in (*.bat) do (
    set /a i+=1
    set "file[!i!]=%%f"
)

sort "%fas%"

for /l %%c in (1,1,%i%) do (
    timeout 1
    start "" "!file[%%c]!"
)

sort /r result.txt /o results.txt

exit /b  
>>>>>>> 537e3964713818d18b2bf088ac61db81448d2537
# laba1_sh
