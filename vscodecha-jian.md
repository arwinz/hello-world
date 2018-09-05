Bracket Pair Colorizer

Clipboard History

Color Info

Copy filename

Debugger for Chrome

Electron Color Theme

Image preview

Local History

open in browser

Relative Path

Subtle Match Brackets

SVG Viewer

function downloadFile\(fileName, content\) {

            var blob = new Blob\(\[content\]\);

            if \(isIe\(\)\)

                window.navigator.msSaveOrOpenBlob\(blob, fileName\);

            else {

                var aLink = document.createElement\("a"\);

                var evt = document.createEvent\("MouseEvents"\);

                evt.initMouseEvent\("click", !0, !0, window, 0, 0, 0, 0, 0, !1, !1, !1, !1, 0, aLink\);

                aLink.download = fileName;

                aLink.href = URL.createObjectURL\(blob\);

                aLink.dispatchEvent\(evt\)

            }

        }

