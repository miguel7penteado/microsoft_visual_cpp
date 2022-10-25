# microsoft_visual_cpp
Compilador Microsoft C++ 32bits e 64 bits

| MSC version | _MSC_VER                                      | Observação |
|-------------|-----------------------------------------------|------------|
| 1.0         | 100 (Microsoft C )                             | 16 bits    |
| 2.0         | 200 (Microsoft C )                             | 16 bits    |
| 3.0         | 300 (Microsoft C )                             | 16 bits    |
| 4.0         | 400 (Microsoft C )                             | 16 bits    |
| 5.0         | 500 (Microsoft C )                             | 16 bits    |
| 6.0         | 600 (Microsoft C )                             | 16 bits    |
| 7.0         | 700 (Microsoft C )                             | 16 bits    |
| 1.0         | 800 (Visual C++ )                             | 32 bits    |
| 2.0         | 900 (Visual C++ )                             | 32 bits    |
| 4.0         | 1000 (Visual Studio 4.0)                      | 32 bits    |
| 4.2         | 1020 (Visual Studio 4.2)                      | 32 bits    |
| 5.0         | 1100 (Visual Studio 5.0)                      | 32 bits    |
| 6.0         | 1200 (Visual Studio 6.0)                      | 32 bits    |
| 7.0         | 1300 (Visual Studio 2002 7.0)                 | 32 bits    |
| 7.1         | 1310 (Visual Studio 2003 7.1)                 | 32 bits    |
| 8.0         | 1400 (Visual Studio 2005 8.0)                 | 32/64 bits |
| 9.0         | 1500 (Visual Studio 2008 9.0)                 | 32/64 bits |
| 10.0        | 1600 (Visual Studio 2010 10.0)                | 32/64 bits |
| 11.0        | 1700 (Visual Studio 2012 11.0)                | 32/64 bits |
| 12.0        | 1800 (Visual Studio 2013 12.0)                | 32/64 bits |
| 14.0        | 1900 (Visual Studio 2015 14.0)                | 32/64 bits |
| 14.1        | 1910 (Visual Studio 2017s 15.0 + 15.1 + 15.2) | 32/64 bits |
| 14.11       | 1911 (Visual Studio 2017 15.3)                | 32/64 bits |
| 14.12       | 1912 (Visual Studio 2017 15.5)                | 32/64 bits |
| 14.13       | 1913 (Visual Studio 2017 15.6)                | 32/64 bits |
| 14.14       | 1914 (Visual Studio 2017 15.7)                | 32/64 bits |
| 14.15       | 1915 (Visual Studio 2017 15.8)                | 32/64 bits |
| 14.16       | 1916 (Visual Studio 2017 15.9)                | 32/64 bits |
| 14.20       | 1920 (Visual Studio 2019 16.0)                | 32/64 bits |
| 14.21       | 1921 (Visual Studio 2019 16.1)                | 32/64 bits |
| 14.22       | 1922 (Visual Studio 2019 16.2)                | 32/64 bits |
| 14.23       | 1923 (Visual Studio 2019 16.3)                | 32/64 bits |
| 14.24       | 1924 (Visual Studio 2019 16.4)                | 32/64 bits |
| 14.25       | 1925 (Visual Studio 2019 16.5)                | 32/64 bits |
| 14.26       | 1926 (Visual Studio 2019 16.6)                | 32/64 bits |
| 14.27       | 1927 (Visual Studio 2019 16.7)                | 32/64 bits |
| 14.28       | 1928 (Visual Studio 2019s 16.8 + 16.9)        | 32/64 bits |
| 14.29       | 1929 (Visual Studio 2019s 16.10 + 16.11)      | 32/64 bits |
| 14.30       | 1930 (Visual Studio 2022 17.0)                | 64 bits    |
| 14.31       | 1931 (Visual Studio 2022 17.1)                | 64 bits    |
| 14.32       | 1932 (Visual Studio 2022 17.2)                | 64 bits    |
| 14.33       | 1933 (Visual Studio 2022 17.3)                | 64 bits    |
| 14.34       | 1934 (Visual Studio 2022 17.4)                | 64 bits    |


setando compiladores e ferramentas de desenvolvimento na raça sem depender de IDE

```cmd
;; ====================================================================================================
;;  INSTALAÇÃO DO CMAKE ULTIMA VERSÃO
;; ====================================================================================================
;wget https://github.com/Kitware/CMake/releases/download/v3.23.0-rc3/cmake-3.23.0-rc3-windows-x86_64.msi
;wget https://github.com/Kitware/CMake/releases/download/v3.25.0-rc1/cmake-3.25.0-rc1-windows-x86_64.zip

;; ====================================================================================================
;;  INSTALAÇÃO DO NINJA ULTIMA VERSÃO
;; ====================================================================================================
;wget https://github.com/ninja-build/ninja/releases/download/v1.10.2/ninja-win.zip

;; ====================================================================================================
;;  INSTALAÇÃO DO WIX ULTIMA VERSÃO
;; ====================================================================================================

;wget https://github.com/wixtoolset/wix3/releases/download/wix3112rtm/wix311.exe
;wget https://github.com/wixtoolset/wix3/releases/download/wix3112rtm/wix311-binaries.zip

;; ====================================================================================================
;;  definição de variáveis do perl
;; ====================================================================================================
set PERL_BASE=F:\perl\straussberry\5.32.1.1\perl
set PERL5LIB=%PERL_BASE%\lib\perl5
set PERL_MM_OPT="INSTALL_BASE=%PERL_BASE%"
set PERL_MB_OPT="--install_base %PERL_BASE%"

;; ====================================================================================================
;;  definição de variáveis base do windows
;; ====================================================================================================
set SystemRoot=C:\WINDOWS
set __VSCMD_PREINIT_PATH=%PATH%
;;=============================================================== 
;; Versionamento para as ferramentas de linha de comando 
;; do visual c++
;;=============================================================== 


set CommandPromptType=Native
set Platform=x64
set VisualStudioVersion=17.0
set VSCMD_ARG_app_plat=Desktop
set VSCMD_ARG_HOST_ARCH=x64
set VSCMD_ARG_TGT_ARCH=x64
set CommandPromptType="Native"
set Platform="x64"
set VisualStudioVersion="17.0"
set VSCMD_ARG_app_plat="Desktop"
set VSCMD_ARG_HOST_ARCH="x64"
set VSCMD_ARG_TGT_ARCH="x64"
set VSCMD_VER="17.1.0"
set __DOTNET_ADD_64BIT="1"
set __DOTNET_PREFERRED_BITNESS="64"

set FrameworkVersion=v4.0.30319
set FrameworkVersion64=v4.0.30319
set WindowsSDKLibVersion=10.0.19041.0
set WindowsSDKVersion=10.0.19041.0
set UCRTVersion=10.0.19041.0
set VCToolsVersion=14.31.31103

;;=============================================================== 
;; Locais de instalação dos softwares auxiliares dos compiladores
;;=============================================================== 

; local de instalação do CMAKE
;set CMAKE_HOME=%ProgramFiles%\CMake
set CMAKE_HOME=F:\cpp\cmake-3.25.0-rc1-windows-x86_64

; local de instalação do NINJA
set NINJA_HOME=F:\cpp\ninja\1.10.2\

; local de instalação do WIX
set WIX=%ProgramFiles(x86)%\WiX Toolset v3.11\

; .NET Framework
set FrameworkDir=F:\cpp\Microsoft.NET\Framework64

; Instalação do Visual Studio
set VSINSTALLDIR=F:\cpp\Microsoft Visual Studio\2022\BuildTools

; Instalação do Visual C++
set VCINSTALLDIR=%VSINSTALLDIR%\VC

; Instalação do Windows SDK
set WindowsSdkDir=F:\cpp\Windows Kits\10

; Instalação das extensões do SDK do windows 10
set ExtensionSdkDir=%WindowsSdkDir%\ExtensionSDKs

;;=============================================================== 

;312 MB
set Framework40Version=v4.0
set FrameworkDir64=%SystemRoot%\Microsoft.NET\Framework64

; 3GB
set DevEnvDir=%VSINSTALLDIR%\Common7\IDE
set VCIDEInstallDir=%DevEnvDir%\VC
set VS170COMNTOOLS=%VSINSTALLDIR%\Common7\Tools

set VCToolsInstallDir=%VCINSTALLDIR%\Tools\MSVC\%VCToolsVersion%
set VCToolsRedistDir=%VCINSTALLDIR%\Redist\MSVC\%VCToolsVersion%

; 2.51 GB

set UniversalCRTSdkDir=%WindowsSdkDir%
set WindowsSdkBinPath=%WindowsSdkDir%\bin
set WindowsSdkVerBinPath=%WindowsSdkDir%\bin\%WindowsSDKVersion%
set WindowsLibPath=%WindowsSdkDir%\UnionMetadata\%WindowsSDKVersion%;%WindowsSdkDir%\References\%WindowsSDKVersion%

;========================================================================
; locais dos arquivos cabeçalho 
;========================================================================
set INCLUDE=%VCToolsInstallDir%\include;%WindowsSdkDir%\include\%UCRTVersion%\ucrt;%WindowsSdkDir%\include\%UCRTVersion%\shared;%WindowsSdkDir%\include\%UCRTVersion%\um;%WindowsSdkDir%\include\%UCRTVersion%\winrt;%WindowsSdkDir%\include\%UCRTVersion%\cppwinrt

;========================================================================
; locais das bibliotecas estáticas 
;========================================================================
set LIB=%VCToolsInstallDir%\lib\x64;%WindowsSdkDir%\lib\%UCRTVersion%\ucrt\x64;%WindowsSdkDir%\lib\%UCRTVersion%\um\x64
set LIBPATH=%VCToolsInstallDir%\lib\x64;%VCToolsInstallDir%\lib\x86\store\references;%WindowsSdkDir%\UnionMetadata\%UCRTVersion%;%WindowsSdkDir%\References\%UCRTVersion%;%FrameworkDir64%\%FrameworkVersion64%


;;=======================================================================
;; ADIOCIONANDO FERRAMENTAS CPP ao PATH
;;=======================================================================

set Path=%SystemRoot%\system32\
set Path=%Path%;%SystemRoot%\
set Path=%Path%;%SystemRoot%\System32\Wbem\
set Path=%Path%;%SystemRoot%\System32\WindowsPowerShell\v1.0\
set Path=%Path%;%SystemRoot%\System32\OpenSSH\

set Path=%Path%;%CMAKE_HOME%\bin\

set Path=%Path%;%VCINSTALLDIR%\Tools\MSVC\%VCToolsVersion%\bin\HostX64\x64\

set Path=%Path%;%VSINSTALLDIR%\Common7\IDE\
set Path=%Path%;%VSINSTALLDIR%\Common7\IDE\CommonExtensions\Microsoft\TestWindow\
set Path=%Path%;%VSINSTALLDIR%\Common7\IDE\CommonExtensions\Microsoft\TeamFoundation\Team Explorer\
;set Path=%Path%;%VSINSTALLDIR%\Common7\IDE\CommonExtensions\Microsoft\CMake\CMake\bin\
;set Path=%Path%;%VSINSTALLDIR%\Common7\IDE\CommonExtensions\Microsoft\CMake\Ninja\
set Path=%Path%;%VSINSTALLDIR%\Common7\IDE\VC\VCPackages\
set Path=%Path%;%VSINSTALLDIR%\Common7\IDE\VC\Linux\bin\ConnectionManagerExe\
set Path=%Path%;%VSINSTALLDIR%\Common7\Tools\
set Path=%Path%;%VSINSTALLDIR%\MSBuild\Current\bin\Roslyn\
set Path=%Path%;%VSINSTALLDIR%\MSBuild\Current\Bin\amd64\

set Path=%Path%;%WindowsSdkDir%\bin\%WindowsSDKVersion%\x64\
set Path=%Path%;%WindowsSdkDir%\bin\x64\
set Path=%Path%;%FrameworkDir64%\%FrameworkVersion64%

;;=======================================================================
;; ADIOCIONANDO FERRAMENTAS JAVA ao PATH
;;=======================================================================
set Path=%Path%;C:\Program Files\Common Files\Oracle\Java\javapath\

;;=======================================================================
;; ADIOCIONANDO FERRAMENTAS PERL ao PATH
;;=======================================================================
set Path=%Path%;%PERL_BASE%\bin
set Path=%Path%;%PERL_BASE%\..\c\bin
set Path=%Path%;%PERL_BASE%\site\bin
set TERM=dumb

;;=======================================================================
;; ADIOCIONANDO FERRAMENTAS TCL ao PATH
;;=======================================================================
set Path=%Path%;C:\ActiveTcl\bin\

;;=======================================================================
;; ADIOCIONANDO FERRAMENTAS GNU linha de comando ao PATH
;;=======================================================================
set Path=%Path%;%ProgramFiles%\Git\cmd\
set Path=%Path%;C:\GnuWin32\bin\
set Path=%Path%;%ProgramFiles%\PuTTY\
set Path=%Path%;%ProgramFiles%\ImageMagick-7.1.0-Q16-HDRI\

set Path=%Path%;%ProgramFiles(x86)%\Common Files\Intel\Shared Libraries\redist\intel64\compiler\
set Path=%Path%;%ProgramFiles%\Docker\Docker\resources\bin\

set Path=%Path%;%ProgramFiles%\MIT\Kerberos\bin\

```
