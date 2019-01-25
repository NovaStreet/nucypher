NuCypher
========
*A proxy re-encryption network to empower privacy in decentralized systems*

.. figure:: data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTAyNCIgaGVpZ2h0PSIxMDI0IiB2aWV3Qm94PSIwIDAgMTAyNCAxMDI0IiB2ZXJzaW9uPSIxLjEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiPgo8dGl0bGU+RGVza3RvcCA0PC90aXRsZT4KPGRlc2M+Q3JlYXRlZCB1c2luZyBGaWdtYTwvZGVzYz4KPGcgaWQ9IkNhbnZhcyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoLTM3NjggMzI5NCkiPgo8Y2xpcFBhdGggaWQ9ImNsaXAtMCIgY2xpcC1ydWxlPSJldmVub2RkIj4KPHBhdGggZD0iTSAzNzY4IC0zMjk0TCA0NzkyIC0zMjk0TCA0NzkyIC0yMjcwTCAzNzY4IC0yMjcwTCAzNzY4IC0zMjk0WiIgZmlsbD0iI0ZGRkZGRiIvPgo8L2NsaXBQYXRoPgo8ZyBpZD0iRGVza3RvcCA0IiBjbGlwLXBhdGg9InVybCgjY2xpcC0wKSI+CjxwYXRoIGQ9Ik0gMzc2OCAtMzI5NEwgNDc5MiAtMzI5NEwgNDc5MiAtMjI3MEwgMzc2OCAtMjI3MEwgMzc2OCAtMzI5NFoiIGZpbGw9IiNGRkZGRkYiLz4KPGcgaWQ9IndvcmRtYXJrIj4KPGcgaWQ9IlZlY3RvciI+Cjx1c2UgeGxpbms6aHJlZj0iI3BhdGgwX2ZpbGwiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDM5MDEgLTI2MjQuNjQpIiBmaWxsPSIjMUU2NUYzIi8+CjwvZz4KPGcgaWQ9IlZlY3RvciI+Cjx1c2UgeGxpbms6aHJlZj0iI3BhdGgxX2ZpbGwiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQwMTYuMzQgLTI1OTAuMjMpIiBmaWxsPSIjMUU2NUYzIi8+CjwvZz4KPGcgaWQ9IlZlY3RvciI+Cjx1c2UgeGxpbms6aHJlZj0iI3BhdGgyX2ZpbGwiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQxMDcuMjUgLTI2MjcpIiBmaWxsPSIjMTIxMTEyIi8+CjwvZz4KPGcgaWQ9IlZlY3RvciI+Cjx1c2UgeGxpbms6aHJlZj0iI3BhdGgzX2ZpbGwiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQyMjQuMjkgLTI1OTAuMjUpIiBmaWxsPSIjMTIxMTEyIi8+CjwvZz4KPGcgaWQ9IlZlY3RvciI+Cjx1c2UgeGxpbms6aHJlZj0iI3BhdGg0X2ZpbGwiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQzMjIuMzMgLTI1OTIuNTkpIiBmaWxsPSIjMTIxMTEyIi8+CjwvZz4KPGcgaWQ9IlZlY3RvciI+Cjx1c2UgeGxpbms6aHJlZj0iI3BhdGg1X2ZpbGwiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ0MjMuMzUgLTI2MjQuNjgpIiBmaWxsPSIjMTIxMTEyIi8+CjwvZz4KPGcgaWQ9IlZlY3RvciI+Cjx1c2UgeGxpbms6aHJlZj0iI3BhdGg2X2ZpbGwiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ1MTIuNTQgLTI1OTIuNjEpIiBmaWxsPSIjMTIxMTEyIi8+CjwvZz4KPGcgaWQ9IlZlY3RvciI+Cjx1c2UgeGxpbms6aHJlZj0iI3BhdGg3X2ZpbGwiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ2MTAuMzYgLTI1OTIuNTkpIiBmaWxsPSIjMTIxMTEyIi8+CjwvZz4KPC9nPgo8ZyBpZD0iY29pbm1hcmsiPgo8ZyBpZD0iVmVjdG9yIj4KPHVzZSB4bGluazpocmVmPSIjcGF0aDhfZmlsbCIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMzk2NCAtMzEzNikiIGZpbGw9IiMxRTY1RjMiLz4KPC9nPgo8L2c+CjwvZz4KPC9nPgo8ZGVmcz4KPHBhdGggaWQ9InBhdGgwX2ZpbGwiIGQ9Ik0gLTEuOTI3MjRlLTA2IDEuNTQxNTNlLTA1TCAxOC41MDM1IDEuNTQxNTNlLTA1TCA3MS40ODc4IDgyLjMxNDdDIDczLjMzNDYgODUuMjAxNCA3NS4wMjEyIDg4LjE4NzYgNzYuNTM5OSA5MS4yNTk2TCA3Ni41Mzk5IDEuNTQxNTNlLTA1TCA5NC4wOTYxIDEuNTQxNTNlLTA1TCA5NC4wOTYxIDExOC4wNzNMIDc1LjUyOTUgMTE4LjA3M0wgMjIuNzEzNiAzNS43NTg4QyAyMC44NjY3IDMyLjg3MiAxOS4xODAxIDI5Ljg4NTkgMTcuNjYxNCAyNi44MTM4TCAxNy42NjE0IDExOC4wNzNMIC0xLjkyNzI0ZS0wNiAxMTguMDczTCAtMS45MjcyNGUtMDYgMS41NDE1M2UtMDVaIi8+CjxwYXRoIGlkPSJwYXRoMV9maWxsIiBkPSJNIDIuOTkxNDdlLTE0IC0zLjg1MzgxZS0wNkwgMTcuMjE5NCAtMy44NTM4MWUtMDZMIDE3LjIxOTQgNTAuMjYwMUMgMTcuMjE5NCA2My4yNDYxIDIzLjk1NTYgNzAuMTcwNiAzNS43NjUgNzAuMTcwNkMgNDguMDc5NSA3MC4xNzA2IDU3LjY5OTcgNTkuNjQ3MSA1Ny42OTk3IDQ1LjIwODlMIDU3LjY5OTcgLTMuODUzODFlLTA2TCA3NC45MTkgLTMuODUzODFlLTA2TCA3NC45MTkgODMuNjYxN0wgNTcuNjk5NyA4My42NjE3TCA1Ny42OTk3IDcwLjE0OTVDIDU1LjEwOTkgNzUuMDY3MSA1MS4xOTIgNzkuMTU5MyA0Ni4zOTE1IDgxLjk2MUMgNDEuNTkxIDg0Ljc2MjcgMzYuMTAwNSA4Ni4xNjEzIDMwLjU0NDQgODUuOTk3OUMgMTQuMTY3IDg1Ljk5NzkgMi45OTE0N2UtMTQgNzUuODc0MyAyLjk5MTQ3ZS0xNCA1My43OTYxTCAyLjk5MTQ3ZS0xNCAtMy44NTM4MWUtMDZaIi8+CjxwYXRoIGlkPSJwYXRoMl9maWxsIiBkPSJNIDExMC4xNTggOTEuNzY0N0MgOTcuODQzMSAxMTEuODIyIDg0LjAxMjkgMTIyLjc4OCA1OC41NDE3IDEyMi43ODhDIDI0Ljk2NiAxMjIuNzg4IDUuMTM5M2UtMDYgOTcuNTMxNiA1LjEzOTNlLTA2IDYxLjM5NEMgNS4xMzkzZS0wNiAyNS4yNTYzIDI2LjY1IC02LjQyMzAyZS0wNiA1OS4zODM3IC02LjQyMzAyZS0wNkMgODMuNTA3NyAtNi40MjMwMmUtMDYgMTAxLjcxNiAxMi42MjgyIDEwOS45MDUgMzAuNTE4MUwgOTUuNDAxMiA0MS4wNDE2QyA4Ni45ODEgMjQuNjg4MSA3NS4zMTkgMTYuNTg1IDU5LjEzMTEgMTYuNTg1QyAzNi44NTk2IDE2LjU4NSAxOC42Mjk4IDM1LjUyNzMgMTguNjI5OCA2MS40NTcxQyAxOC42Mjk4IDg3LjA5MjMgMzUuNjgwNyAxMDYuMzI5IDU4Ljk2MjcgMTA2LjMyOUMgNzQuODEzOCAxMDYuMzI5IDg3LjI5NjggOTguNzMxMyA5Ni4yNDMzIDgxLjg3MjdMIDExMC4xNTggOTEuNzY0N1oiLz4KPHBhdGggaWQ9InBhdGgzX2ZpbGwiIGQ9Ik0gMTIuNDgzIDEwMS43NDFDIDE0Ljg4MzIgMTAyLjc4OSAxNy40NjQgMTAzLjM2MSAyMC4wODIzIDEwMy40MjVDIDI0LjQ2MDggMTAzLjQyNSAyNy4xNTUzIDEwMi4wNzggMzAuMjA3NiA5NC40Nzk4TCAzNC4wODA5IDg0LjE4NzlMIC0xLjQxMzMxZS0wNSA3LjcwNzYzZS0wNkwgMTkuNzQ1NCA3LjcwNzYzZS0wNkwgNDMuMzY0MiA2MC4zODM4TCA2Ni44MTQ1IDcuNzA3NjNlLTA2TCA4NS43NjAxIDcuNzA3NjNlLTA2TCA0NS4yNzk4IDEwMC41NDFDIDM5Ljg5MDkgMTE0LjIwMSAzMS45NTQ4IDExOS4yNTIgMjEuODI5NSAxMTkuMjUyQyAxNy43MTA1IDExOS4yNTEgMTMuNjE1NCAxMTguNjI2IDkuNjgzMjcgMTE3LjRMIDEyLjQ4MyAxMDEuNzQxWiIvPgo8cGF0aCBpZD0icGF0aDRfZmlsbCIgZD0iTSAtMy4wODM1OGUtMDUgMi4zNTcyNkwgMTcuMTk4MyAyLjM1NzI2TCAxNy4xOTgzIDE1LjE3NDhDIDIyLjQzOTkgNi45MDMzOSAzMy45MTI1IDYuNDIzMDJlLTA2IDQ2LjkwMDcgNi40MjMwMmUtMDZDIDY3LjgwNCA2LjQyMzAyZS0wNiA4NS41Mjg1IDE2LjUyMTkgODUuNTI4NSA0NC4xOTg2QyA4NS41Mjg1IDcxLjM0OTIgNjcuODA0IDg4LjM5NzIgNDUuMzg1MSA4OC4zOTcyQyAzMy4zODYyIDg4LjM5NzIgMjIuNTg3MyA4My4wMDkyIDE3LjE5ODMgNzQuNTY5NEwgMTcuMTk4MyAxMjAuNDUyTCAtMy4wODM1OGUtMDUgMTIwLjQ1MkwgLTMuMDgzNThlLTA1IDIuMzU3MjZaTSAxNi4wODI2IDQ0LjE5ODZDIDE2LjA4MjYgNjEuMDM2MiAyNy43MjM2IDcyLjUyNzkgNDIuMDU5MSA3Mi41Mjc5QyA1Ni4zOTQ1IDcyLjUyNzkgNjguMDM1NSA2MS4wNTcyIDY4LjAzNTUgNDQuMTk4NkMgNjguMDM1NSAyNy4zNCA1Ni4zOTQ1IDE1Ljg0ODQgNDIuMDU5MSAxNS44NDg0QyAyNy43MjM2IDE1Ljg0ODQgMTYuMDgyNiAyNy4zMTkgMTYuMDgyNiA0NC4xOTg2WiIvPgo8cGF0aCBpZD0icGF0aDVfZmlsbCIgZD0iTSA3NS45MDg0IDExOC4xMTZMIDU4LjcxMDEgMTE4LjExNkwgNTguNzEwMSA2Ni44NDUxQyA1OC43MTAxIDU0Ljg2OTQgNTEuNjE2MSA0Ny45MDI5IDQwLjE0MzUgNDcuOTAyOUMgMjcuODI4OSA0Ny45MDI5IDE3LjE5ODMgNTguMDI2NSAxNy4xOTgzIDczLjg3NDhMIDE3LjE5ODMgMTE4LjA3M0wgMS4yODQ4M2UtMDUgMTE4LjA3M0wgMS4yODQ4M2UtMDUgNi40MjMwMmUtMDZMIDE3LjE5ODMgNi40MjMwMmUtMDZMIDE3LjE5ODMgNDguNDA4QyAyMC4yNjUyIDQzLjQ1NiAyNC41MzQ5IDM5LjM1OTkgMjkuNjEwMyAzNi41MDA2QyAzNC42ODU2IDMzLjY0MTQgNDAuNDAxOCAzMi4xMTE5IDQ2LjIyNzEgMzIuMDU0NUMgNjIuNTgzNCAzMi4wNTQ1IDc1LjkwODQgNDIuMzQ2NSA3NS45MDg0IDYxLjUyMDNMIDc1LjkwODQgMTE4LjExNloiLz4KPHBhdGggaWQ9InBhdGg2X2ZpbGwiIGQ9Ik0gMTcuMTM1MSA0Ny45MjM5QyAxNy44MDg4IDYyLjc2MiAyNy43NjU3IDczLjM5MDggNDIuNjA2NCA3My4zOTA4QyA1Ni4yNjgyIDczLjM5MDggNjIuNjg4NyA2NS45NjEyIDY3LjU3MjQgNTYuMDA2TCA4MC44OTc0IDYzLjk0MDdDIDczLjE1MDggNzkuOTU3NCA2MC45ODM1IDg4LjM5NzMgNDIuMTAxMiA4OC4zOTczQyAxOS4xNTYgODguMzk3MyAyLjU2OTY1ZS0wNiA3MC4zNiAyLjU2OTY1ZS0wNiA0NC4xOTg2QyAyLjU2OTY1ZS0wNiAxOC4wMzcyIDE5LjI0MDIgLTEuNDEzMDdlLTA1IDQzLjAyNzQgLTEuNDEzMDdlLTA1QyA2Ny4zMTk4IC0xLjQxMzA3ZS0wNSA4My41Mjg3IDE3LjM2MzggODMuNTI4NyA0MS44MjAzTCA4My41Mjg3IDQ3LjkwMjlMIDE3LjEzNTEgNDcuOTIzOVpNIDE3LjEzNTEgMzQuNzY5NkwgNjcuMDY3MSAzNC43Njk2QyA2NS43MTk5IDIxLjExMDEgNTQuMjQ3MyAxMy44NDg5IDQyLjYwNjQgMTMuODQ4OUMgMzAuMDYwMiAxMy44NDg5IDIwLjMzNDggMjIuNjI1NSAxNy4xMzUxIDM0Ljc2OTZaIi8+CjxwYXRoIGlkPSJwYXRoN19maWxsIiBkPSJNIDQ0LjY5MDQgMTcuMTk1NEMgNDIuNTY3MSAxNi41MTg5IDQwLjM1MTEgMTYuMTc4IDM4LjEyMjYgMTYuMTg1MUMgMjUuOTc2NCAxNi4xODUxIDE3LjE5ODMgMjcuMTUwNiAxNy4xOTgzIDQxLjk4ODdMIDE3LjE5ODMgODYuMDE5TCA1LjEzOTNlLTA2IDg2LjAxOUwgNS4xMzkzZS0wNiAyLjM1NzI2TCAxNy4xOTgzIDIuMzU3MjZMIDE3LjE5ODMgMTYuNTIxOUMgMjEuNzQ1MiA2LjczNTAxIDI5LjgyODcgNi40MjMwMmUtMDYgNDEuMzIyMyA2LjQyMzAyZS0wNkMgNDMuNDUzNCAwLjAyNzk0NjcgNDUuNTczNSAwLjMxMDU2NiA0Ny42Mzc1IDAuODQxODcyTCA0NC42OTA0IDE3LjE5NTRaIi8+CjxwYXRoIGlkPSJwYXRoOF9maWxsIiBkPSJNIDQ0Mi43NTIgMC4xOTU0MjJMIDM5NC40ODcgMjMuMDk1M0MgMzk0LjI0MiAyMy4yMTExIDM5NC4wMjIgMjMuMzc0MSAzOTMuODM5IDIzLjU3NTFDIDM5My42NTcgMjMuNzc2MiAzOTMuNTE2IDI0LjAxMTIgMzkzLjQyNCAyNC4yNjY4QyAzOTMuMzMzIDI0LjUyMjMgMzkzLjI5MyAyNC43OTM1IDM5My4zMDYgMjUuMDY0NkMgMzkzLjMyIDI1LjMzNTcgMzkzLjM4NyAyNS42MDE0IDM5My41MDMgMjUuODQ2N0wgNDY2LjkwOCAxODAuNTg0QyA0OTQuMTgzIDIzOC4xNDggNDg2Ljg3OCAyODEuODE0IDQ0NS40MDggMzAxLjU0N0MgNDExLjg0OCAzMTcuNDc0IDM4Mi44NzggMzA2LjM2MiAzNjAuMjc1IDI2Ny41NTlMIDI3My4zNjMgODQuMzM1OEMgMjM4LjExOSAxMC4wNjIyIDE5MC4xMTUgLTkuNjIzOTIgMTMzLjE3IDE3LjM5MTFDIDk2LjEyMzcgMzQuOTY2MyA3NC42MzU4IDY2LjM4MTEgNzUuMDYyNyAxMDYuMjUxQyA3NS4wNzEgMTA2LjcyMiA3NC45MTc4IDEwNy4xODIgNzQuNjI4NSAxMDcuNTU0QyA3NC4zMzkzIDEwNy45MjYgNzMuOTMxNSAxMDguMTg4IDczLjQ3MjkgMTA4LjI5NkMgNzMuMDE0MyAxMDguNDA0IDcyLjUzMjYgMTA4LjM1MiA3Mi4xMDc3IDEwOC4xNDhDIDcxLjY4MjkgMTA3Ljk0NSA3MS4zNDA1IDEwNy42MDIgNzEuMTM3NSAxMDcuMTc2TCA1Mi4xNjM3IDY3LjE5OTNDIDUyLjA0ODEgNjYuOTUzOCA1MS44ODUgNjYuNzMzNiA1MS42ODM3IDY2LjU1MTVDIDUxLjQ4MjQgNjYuMzY5NCA1MS4yNDcgNjYuMjI5MSA1MC45OTExIDY2LjEzODdDIDUwLjczNTIgNjYuMDQ4MiA1MC40NjM5IDY2LjAwOTUgNTAuMTkzIDY2LjAyNDZDIDQ5LjkyMiA2Ni4wMzk3IDQ5LjY1NjcgNjYuMTA4NSA0OS40MTI1IDY2LjIyNjlMIDEuMTU5NjQgODkuMDU1N0MgMC42NzU3OTIgODkuMjg5MyAwLjMwMjg4NiA4OS43MDMzIDAuMTIxMDU3IDkwLjIwODlDIC0wLjA2MDc3MjYgOTAuNzE0NSAtMC4wMzcwMTMyIDkxLjI3MTMgMC4xODcyMjkgOTEuNzU5NkwgMTMzLjQ3OCAzNzIuODJDIDEzMy43MTUgMzczLjMxNCAxMzQuMTM2IDM3My42OTQgMTM0LjY1MSAzNzMuODc5QyAxMzUuMTY3IDM3NC4wNjMgMTM1LjczNCAzNzQuMDM2IDEzNi4yMyAzNzMuODA1TCAxODQuNDk0IDM1MC45MDVDIDE4NC43NCAzNTAuNzg5IDE4NC45NiAzNTAuNjI2IDE4NS4xNDMgMzUwLjQyNUMgMTg1LjMyNSAzNTAuMjI0IDE4NS40NjYgMzQ5Ljk4OSAxODUuNTU3IDM0OS43MzNDIDE4NS42NDkgMzQ5LjQ3OCAxODUuNjg5IDM0OS4yMDcgMTg1LjY3NSAzNDguOTM1QyAxODUuNjYyIDM0OC42NjQgMTg1LjU5NSAzNDguMzk5IDE4NS40NzkgMzQ4LjE1M0wgMTE0LjEyNSAxOTcuNzQ0QyA4NS4wNTk2IDEzNi40NTYgOTAuNTczOSA5Mi4xMzkgMTM1LjEzOSA3MC45OTQzQyAxNjkuMzM5IDU0Ljc3MSAxOTUuOTI2IDY1LjY4MTQgMjE5Ljc5OCAxMDcuMjQ4QyAyMTkuODMgMTA3LjI5NiAyMTkuODU4IDEwNy4zNDggMjE5Ljg4MSAxMDcuNDAyTCAzMDUuOTM5IDI4OC44NDZDIDMzOS4xNDMgMzU4LjgxNSAzOTAuNzE2IDM4Mi44NDEgNDQ1LjE4MyAzNTdDIDQ4Ny4yODEgMzM3LjAzIDUwNC43MzcgMzA2Ljk2NyA1MDMuNzE3IDI2Ny40MjhDIDUwMy43MDYgMjY2Ljk1NiA1MDMuODU3IDI2Ni40OTUgNTA0LjE0NiAyNjYuMTJDIDUwNC40MzQgMjY1Ljc0NiA1MDQuODQyIDI2NS40ODMgNTA1LjMwMSAyNjUuMzczQyA1MDUuNzYxIDI2NS4yNjMgNTA2LjI0NCAyNjUuMzE0IDUwNi42NyAyNjUuNTE4QyA1MDcuMDk2IDI2NS43MjIgNTA3LjQzOSAyNjYuMDY1IDUwNy42NDMgMjY2LjQ5MkwgNTI2LjgwNiAzMDYuODk2QyA1MjYuOTIyIDMwNy4xNDEgNTI3LjA4NSAzMDcuMzYxIDUyNy4yODYgMzA3LjU0NEMgNTI3LjQ4NyAzMDcuNzI2IDUyNy43MjIgMzA3Ljg2NyA1MjcuOTc4IDMwNy45NTlDIDUyOC4yMzMgMzA4LjA1IDUyOC41MDQgMzA4LjA5IDUyOC43NzUgMzA4LjA3N0MgNTI5LjA0NiAzMDguMDYzIDUyOS4zMTIgMzA3Ljk5NiA1MjkuNTU3IDMwNy44OEwgNTc3LjgyMiAyODQuOThDIDU3OC4wNjggMjg0Ljg2NCA1NzguMjg4IDI4NC43MDEgNTc4LjQ3IDI4NC41QyA1NzguNjUyIDI4NC4yOTkgNTc4Ljc5MiAyODQuMDYzIDU3OC44ODMgMjgzLjgwN0MgNTc4Ljk3MyAyODMuNTUxIDU3OS4wMTIgMjgzLjI4IDU3OC45OTcgMjgzLjAwOUMgNTc4Ljk4MiAyODIuNzM4IDU3OC45MTMgMjgyLjQ3MyA1NzguNzk0IDI4Mi4yMjlMIDQ0NS41MDMgMS4xNzk3M0MgNDQ1LjI2NyAwLjY4NjA1IDQ0NC44NDUgMC4zMDU2MyA0NDQuMzMgMC4xMjEyODVDIDQ0My44MTUgLTAuMDYzMDYxNCA0NDMuMjQ4IC0wLjAzNjQxMjkgNDQyLjc1MiAwLjE5NTQyMloiLz4KPC9kZWZzPgo8L3N2Zz4K
    :width: 60%

.. image:: https://img.shields.io/pypi/wheel/nucypher.svg
    :target: https://pypi.org/project/nucypher/

.. image:: https://img.shields.io/pypi/pyversions/nucypher.svg
    :target: https://pypi.org/project/nucypher/

.. image:: https://coveralls.io/repos/github/nucypher/nucypher/badge.svg?branch=master
    :target: https://coveralls.io/github/nucypher/nucypher?branch=master

.. image:: https://circleci.com/gh/nucypher/nucypher/tree/master.svg?style=svg
    :target: https://circleci.com/gh/nucypher/nucypher/tree/master


- GitHub https://www.gihub.com/nucypher/nucypher
- Documentation https://nucypher.readthedocs.io/en/latest/
- Website https://www.nucypher.com/


Whitepapers
-----------

**Network**

    https://www.nucypher.com/static/whitepapers/english.pdf

    *"NuCypher - A proxy re-encryption network to empower privacy in decentralized systems"*
    *by Michael Egorov, David Nuñez, and MacLane Wilkison - NuCypher*


**Economics**

    https://www.nucypher.com/static/whitepapers/mining-paper.pdf

    *"NuCypher - Mining & Staking Economics"*
    *by Michael Egorov, MacLane Wilkison - NuCypher*


**Cryptography**

    https://github.com/nucypher/umbral-doc/blob/master/umbral-doc.pdf

    *"Umbral A Threshold Proxy Re-Encryption Scheme"*
    *by David Nuñez*


.. warning::

   NuCypher is currently in the *Alpha* development stage and is **not** intended for use production.


.. toctree::
   :maxdepth: 2


Architecture
------------

.. toctree::
   :maxdepth: 1

   architecture/contracts
   architecture/upgradeable_proxy_contracts


Guides
------

.. toctree::
   :maxdepth: 2

   guides/quickstart
   guides/ursula_configuration_guide
   guides/federated_testnet_guide
   guides/installation_guide
   guides/contribution_guide


Demos
-----

.. toctree::
   :maxdepth: 2

   demos/local_fleet_demo
   demos/finnegans_wake_demo
   demos/heartbeat_demo


API
---

.. toctree::
   :maxdepth: 2

   api/characters
   api/config
   api/crypto
   api/keyring
   api/keystore
   api/network
   api/policy


Release Notes
-------------

.. toctree::
   :maxdepth: 1

   release_notes/genesis_release


Indices and Tables
==================
* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
