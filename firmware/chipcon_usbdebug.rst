                              1 ;--------------------------------------------------------
                              2 ; File Created by SDCC : free open source ANSI-C Compiler
                              3 ; Version 3.3.0 #8604 (Dec 30 2013) (Linux)
                              4 ; This file was generated Fri Dec 16 14:41:37 2016
                              5 ;--------------------------------------------------------
                              6 	.module chipcon_usbdebug
                              7 	.optsdcc -mmcs51 --model-small
                              8 	
                              9 ;--------------------------------------------------------
                             10 ; Public variables in this module
                             11 ;--------------------------------------------------------
                             12 	.globl _txdata
                             13 	.globl _USBIF
                             14 	.globl _MODE
                             15 	.globl _RE
                             16 	.globl _SLAVE
                             17 	.globl _FE
                             18 	.globl _ERR
                             19 	.globl _RX_BYTE
                             20 	.globl _TX_BYTE
                             21 	.globl _ACTIVE
                             22 	.globl _B_7
                             23 	.globl _B_6
                             24 	.globl _B_5
                             25 	.globl _B_4
                             26 	.globl _B_3
                             27 	.globl _B_2
                             28 	.globl _B_1
                             29 	.globl _B_0
                             30 	.globl _WDTIF
                             31 	.globl _P1IF
                             32 	.globl _UTX1IF
                             33 	.globl _UTX0IF
                             34 	.globl _P2IF
                             35 	.globl _ACC_7
                             36 	.globl _ACC_6
                             37 	.globl _ACC_5
                             38 	.globl _ACC_4
                             39 	.globl _ACC_3
                             40 	.globl _ACC_2
                             41 	.globl _ACC_1
                             42 	.globl _ACC_0
                             43 	.globl _OVFIM
                             44 	.globl _T4CH1IF
                             45 	.globl _T4CH0IF
                             46 	.globl _T4OVFIF
                             47 	.globl _T3CH1IF
                             48 	.globl _T3CH0IF
                             49 	.globl _T3OVFIF
                             50 	.globl _CY
                             51 	.globl _AC
                             52 	.globl _F0
                             53 	.globl _RS1
                             54 	.globl _RS0
                             55 	.globl _OV
                             56 	.globl _F1
                             57 	.globl _P
                             58 	.globl _STIF
                             59 	.globl _P0IF
                             60 	.globl _T4IF
                             61 	.globl _T3IF
                             62 	.globl _T2IF
                             63 	.globl _T1IF
                             64 	.globl _DMAIF
                             65 	.globl _P0IE
                             66 	.globl _T4IE
                             67 	.globl _T3IE
                             68 	.globl _T2IE
                             69 	.globl _T1IE
                             70 	.globl _DMAIE
                             71 	.globl _EA
                             72 	.globl _STIE
                             73 	.globl _ENCIE
                             74 	.globl _URX1IE
                             75 	.globl _URX0IE
                             76 	.globl _ADCIE
                             77 	.globl _RFTXRXIE
                             78 	.globl _P2_7
                             79 	.globl _P2_6
                             80 	.globl _P2_5
                             81 	.globl _P2_4
                             82 	.globl _P2_3
                             83 	.globl _P2_2
                             84 	.globl _P2_1
                             85 	.globl _P2_0
                             86 	.globl _ENCIF_1
                             87 	.globl _ENCIF_0
                             88 	.globl _P1_7
                             89 	.globl _P1_6
                             90 	.globl _P1_5
                             91 	.globl _P1_4
                             92 	.globl _P1_3
                             93 	.globl _P1_2
                             94 	.globl _P1_1
                             95 	.globl _P1_0
                             96 	.globl _URX1IF
                             97 	.globl _ADCIF
                             98 	.globl _URX0IF
                             99 	.globl _IT1
                            100 	.globl _RFTXRXIF
                            101 	.globl _IT0
                            102 	.globl _P0_7
                            103 	.globl _P0_6
                            104 	.globl _P0_5
                            105 	.globl _P0_4
                            106 	.globl _P0_3
                            107 	.globl _P0_2
                            108 	.globl _P0_1
                            109 	.globl _P0_0
                            110 	.globl _P2DIR
                            111 	.globl _P1DIR
                            112 	.globl _P0DIR
                            113 	.globl _U1GCR
                            114 	.globl _U1UCR
                            115 	.globl _U1BAUD
                            116 	.globl _U1DBUF
                            117 	.globl _U1CSR
                            118 	.globl _P2INP
                            119 	.globl _P1INP
                            120 	.globl _P2SEL
                            121 	.globl _P1SEL
                            122 	.globl _P0SEL
                            123 	.globl _ADCCFG
                            124 	.globl _PERCFG
                            125 	.globl _B
                            126 	.globl _T4CC1
                            127 	.globl _T4CCTL1
                            128 	.globl _T4CC0
                            129 	.globl _T4CCTL0
                            130 	.globl _T4CTL
                            131 	.globl _T4CNT
                            132 	.globl _RFIF
                            133 	.globl _IRCON2
                            134 	.globl _T1CCTL2
                            135 	.globl _T1CCTL1
                            136 	.globl _T1CCTL0
                            137 	.globl _T1CTL
                            138 	.globl _T1CNTH
                            139 	.globl _T1CNTL
                            140 	.globl _RFST
                            141 	.globl _ACC
                            142 	.globl _T1CC2H
                            143 	.globl _T1CC2L
                            144 	.globl _T1CC1H
                            145 	.globl _T1CC1L
                            146 	.globl _T1CC0H
                            147 	.globl _T1CC0L
                            148 	.globl _RFD
                            149 	.globl _TIMIF
                            150 	.globl _DMAREQ
                            151 	.globl _DMAARM
                            152 	.globl _DMA0CFGH
                            153 	.globl _DMA0CFGL
                            154 	.globl _DMA1CFGH
                            155 	.globl _DMA1CFGL
                            156 	.globl _DMAIRQ
                            157 	.globl _PSW
                            158 	.globl _T3CC1
                            159 	.globl _T3CCTL1
                            160 	.globl _T3CC0
                            161 	.globl _T3CCTL0
                            162 	.globl _T3CTL
                            163 	.globl _T3CNT
                            164 	.globl _WDCTL
                            165 	.globl __SFRC8
                            166 	.globl _MEMCTR
                            167 	.globl _CLKCON
                            168 	.globl _U0GCR
                            169 	.globl _U0UCR
                            170 	.globl __SFRC3
                            171 	.globl _U0BAUD
                            172 	.globl _U0DBUF
                            173 	.globl _IRCON
                            174 	.globl __SFRBF
                            175 	.globl _SLEEP
                            176 	.globl _RNDH
                            177 	.globl _RNDL
                            178 	.globl _ADCH
                            179 	.globl _ADCL
                            180 	.globl _IP1
                            181 	.globl _IEN1
                            182 	.globl __SFRB7
                            183 	.globl _ADCCON3
                            184 	.globl _ADCCON2
                            185 	.globl _ADCCON1
                            186 	.globl _ENCCS
                            187 	.globl _ENCDO
                            188 	.globl _ENCDI
                            189 	.globl __SFRB0
                            190 	.globl _FWDATA
                            191 	.globl _FCTL
                            192 	.globl _FADDRH
                            193 	.globl _FADDRL
                            194 	.globl _FWT
                            195 	.globl __SFRAA
                            196 	.globl _IP0
                            197 	.globl _IEN0
                            198 	.globl __SFRA7
                            199 	.globl _WORTIME1
                            200 	.globl _WORTIME0
                            201 	.globl _WOREVT1
                            202 	.globl _WOREVT0
                            203 	.globl _WORCTRL
                            204 	.globl _WORIRQ
                            205 	.globl _P2
                            206 	.globl __SFR9F
                            207 	.globl _T2CTL
                            208 	.globl _T2PR
                            209 	.globl _T2CT
                            210 	.globl _S1CON
                            211 	.globl _IEN2
                            212 	.globl __SFR99
                            213 	.globl _S0CON
                            214 	.globl __SFR97
                            215 	.globl __SFR96
                            216 	.globl __SFR95
                            217 	.globl __SFR94
                            218 	.globl __XPAGE
                            219 	.globl _MPAGE
                            220 	.globl _DPS
                            221 	.globl _RFIM
                            222 	.globl _P1
                            223 	.globl _P0INP
                            224 	.globl __SFR8E
                            225 	.globl _P1IEN
                            226 	.globl _PICTL
                            227 	.globl _P2IFG
                            228 	.globl _P1IFG
                            229 	.globl _P0IFG
                            230 	.globl _TCON
                            231 	.globl _PCON
                            232 	.globl _U0CSR
                            233 	.globl _DPH1
                            234 	.globl _DPL1
                            235 	.globl _DPH0
                            236 	.globl _DPL0
                            237 	.globl _SP
                            238 	.globl _P0
                            239 	.globl _USBF5
                            240 	.globl _USBF4
                            241 	.globl _USBF3
                            242 	.globl _USBF2
                            243 	.globl _USBF1
                            244 	.globl _USBF0
                            245 	.globl _USBCNTH
                            246 	.globl _USBCNTL
                            247 	.globl _USBCNT0
                            248 	.globl _USBCSOH
                            249 	.globl _USBCSOL
                            250 	.globl _USBMAXO
                            251 	.globl _USBCSIH
                            252 	.globl _USBCSIL
                            253 	.globl _USBCS0
                            254 	.globl _USBMAXI
                            255 	.globl _USBINDEX
                            256 	.globl _USBFRMH
                            257 	.globl _USBFRML
                            258 	.globl _USBCIE
                            259 	.globl _USBOIE
                            260 	.globl _USBIIE
                            261 	.globl _USBCIF
                            262 	.globl _USBOIF
                            263 	.globl _USBIIF
                            264 	.globl _USBPOW
                            265 	.globl _USBADDR
                            266 	.globl _X_P2DIR
                            267 	.globl _X_P1DIR
                            268 	.globl _X_P0DIR
                            269 	.globl _X_U1GCR
                            270 	.globl _X_U1UCR
                            271 	.globl _X_U1BAUD
                            272 	.globl _X_U1DBUF
                            273 	.globl _X_U1CSR
                            274 	.globl _X_P2INP
                            275 	.globl _X_P1INP
                            276 	.globl _X_P2SEL
                            277 	.globl _X_P1SEL
                            278 	.globl _X_P0SEL
                            279 	.globl _X_ADCCFG
                            280 	.globl _X_PERCFG
                            281 	.globl __NA_B
                            282 	.globl _X_T4CC1
                            283 	.globl _X_T4CCTL1
                            284 	.globl _X_T4CC0
                            285 	.globl _X_T4CCTL0
                            286 	.globl _X_T4CTL
                            287 	.globl _X_T4CNT
                            288 	.globl _X_RFIF
                            289 	.globl __NA_IRCON2
                            290 	.globl _X_T1CCTL2
                            291 	.globl _X_T1CCTL1
                            292 	.globl _X_T1CCTL0
                            293 	.globl _X_T1CTL
                            294 	.globl _X_T1CNTH
                            295 	.globl _X_T1CNTL
                            296 	.globl _X_RFST
                            297 	.globl __NA_ACC
                            298 	.globl _X_T1CC2H
                            299 	.globl _X_T1CC2L
                            300 	.globl _X_T1CC1H
                            301 	.globl _X_T1CC1L
                            302 	.globl _X_T1CC0H
                            303 	.globl _X_T1CC0L
                            304 	.globl _X_RFD
                            305 	.globl _X_TIMIF
                            306 	.globl _X_DMAREQ
                            307 	.globl _X_DMAARM
                            308 	.globl _X_DMA0CFGH
                            309 	.globl _X_DMA0CFGL
                            310 	.globl _X_DMA1CFGH
                            311 	.globl _X_DMA1CFGL
                            312 	.globl _X_DMAIRQ
                            313 	.globl __NA_PSW
                            314 	.globl _X_T3CC1
                            315 	.globl _X_T3CCTL1
                            316 	.globl _X_T3CC0
                            317 	.globl _X_T3CCTL0
                            318 	.globl _X_T3CTL
                            319 	.globl _X_T3CNT
                            320 	.globl _X_WDCTL
                            321 	.globl __X_SFRC8
                            322 	.globl _X_MEMCTR
                            323 	.globl _X_CLKCON
                            324 	.globl _X_U0GCR
                            325 	.globl _X_U0UCR
                            326 	.globl __X_SFRC3
                            327 	.globl _X_U0BAUD
                            328 	.globl _X_U0DBUF
                            329 	.globl __NA_IRCON
                            330 	.globl __X_SFRBF
                            331 	.globl _X_SLEEP
                            332 	.globl _X_RNDH
                            333 	.globl _X_RNDL
                            334 	.globl _X_ADCH
                            335 	.globl _X_ADCL
                            336 	.globl __NA_IP1
                            337 	.globl __NA_IEN1
                            338 	.globl __X_SFRB7
                            339 	.globl _X_ADCCON3
                            340 	.globl _X_ADCCON2
                            341 	.globl _X_ADCCON1
                            342 	.globl _X_ENCCS
                            343 	.globl _X_ENCDO
                            344 	.globl _X_ENCDI
                            345 	.globl __X_SFRB0
                            346 	.globl _X_FWDATA
                            347 	.globl _X_FCTL
                            348 	.globl _X_FADDRH
                            349 	.globl _X_FADDRL
                            350 	.globl _X_FWT
                            351 	.globl __X_SFRAA
                            352 	.globl __NA_IP0
                            353 	.globl __NA_IEN0
                            354 	.globl __X_SFRA7
                            355 	.globl _X_WORTIME1
                            356 	.globl _X_WORTIME0
                            357 	.globl _X_WOREVT1
                            358 	.globl _X_WOREVT0
                            359 	.globl _X_WORCTRL
                            360 	.globl _X_WORIRQ
                            361 	.globl __NA_P2
                            362 	.globl __X_SFR9F
                            363 	.globl _X_T2CTL
                            364 	.globl _X_T2PR
                            365 	.globl _X_T2CT
                            366 	.globl __NA_S1CON
                            367 	.globl __NA_IEN2
                            368 	.globl __X_SFR99
                            369 	.globl __NA_S0CON
                            370 	.globl __X_SFR97
                            371 	.globl __X_SFR96
                            372 	.globl __X_SFR95
                            373 	.globl __X_SFR94
                            374 	.globl _X_MPAGE
                            375 	.globl __NA_DPS
                            376 	.globl _X_RFIM
                            377 	.globl __NA_P1
                            378 	.globl _X_P0INP
                            379 	.globl __X_SFR8E
                            380 	.globl _X_P1IEN
                            381 	.globl _X_PICTL
                            382 	.globl _X_P2IFG
                            383 	.globl _X_P1IFG
                            384 	.globl _X_P0IFG
                            385 	.globl __NA_TCON
                            386 	.globl __NA_PCON
                            387 	.globl _X_U0CSR
                            388 	.globl __NA_DPH1
                            389 	.globl __NA_DPL1
                            390 	.globl __NA_DPH0
                            391 	.globl __NA_DPL0
                            392 	.globl __NA_SP
                            393 	.globl __NA_P0
                            394 	.globl _I2SCLKF2
                            395 	.globl _I2SCLKF1
                            396 	.globl _I2SCLKF0
                            397 	.globl _I2SSTAT
                            398 	.globl _I2SWCNT
                            399 	.globl _I2SDATH
                            400 	.globl _I2SDATL
                            401 	.globl _I2SCFG1
                            402 	.globl _I2SCFG0
                            403 	.globl _VCO_VC_DAC
                            404 	.globl _PKTSTATUS
                            405 	.globl _MARCSTATE
                            406 	.globl _RSSI
                            407 	.globl _LQI
                            408 	.globl _FREQEST
                            409 	.globl _VERSION
                            410 	.globl _PARTNUM
                            411 	.globl __XREGDF35
                            412 	.globl __XREGDF34
                            413 	.globl __XREGDF33
                            414 	.globl __XREGDF32
                            415 	.globl _IOCFG0
                            416 	.globl _IOCFG1
                            417 	.globl _IOCFG2
                            418 	.globl _PA_TABLE0
                            419 	.globl _PA_TABLE1
                            420 	.globl _PA_TABLE2
                            421 	.globl _PA_TABLE3
                            422 	.globl _PA_TABLE4
                            423 	.globl _PA_TABLE5
                            424 	.globl _PA_TABLE6
                            425 	.globl _PA_TABLE7
                            426 	.globl __XREGDF26
                            427 	.globl _TEST0
                            428 	.globl _TEST1
                            429 	.globl _TEST2
                            430 	.globl __XREGDF22
                            431 	.globl __XREGDF21
                            432 	.globl __XREGDF20
                            433 	.globl _FSCAL0
                            434 	.globl _FSCAL1
                            435 	.globl _FSCAL2
                            436 	.globl _FSCAL3
                            437 	.globl _FREND0
                            438 	.globl _FREND1
                            439 	.globl _AGCCTRL0
                            440 	.globl _AGCCTRL1
                            441 	.globl _AGCCTRL2
                            442 	.globl _BSCFG
                            443 	.globl _FOCCFG
                            444 	.globl _MCSM0
                            445 	.globl _MCSM1
                            446 	.globl _MCSM2
                            447 	.globl _DEVIATN
                            448 	.globl _MDMCFG0
                            449 	.globl _MDMCFG1
                            450 	.globl _MDMCFG2
                            451 	.globl _MDMCFG3
                            452 	.globl _MDMCFG4
                            453 	.globl _FREQ0
                            454 	.globl _FREQ1
                            455 	.globl _FREQ2
                            456 	.globl _FSCTRL0
                            457 	.globl _FSCTRL1
                            458 	.globl _CHANNR
                            459 	.globl _ADDR
                            460 	.globl _PKTCTRL0
                            461 	.globl _PKTCTRL1
                            462 	.globl _PKTLEN
                            463 	.globl _SYNC0
                            464 	.globl _SYNC1
                            465 	.globl _MDMCTRL0H
                            466 	.globl _debugx
                            467 	.globl _debug
                            468 	.globl _debughex
                            469 	.globl _debughex16
                            470 	.globl _debughex32
                            471 ;--------------------------------------------------------
                            472 ; special function registers
                            473 ;--------------------------------------------------------
                            474 	.area RSEG    (ABS,DATA)
   0000                     475 	.org 0x0000
                     0080   476 _P0	=	0x0080
                     0081   477 _SP	=	0x0081
                     0082   478 _DPL0	=	0x0082
                     0083   479 _DPH0	=	0x0083
                     0084   480 _DPL1	=	0x0084
                     0085   481 _DPH1	=	0x0085
                     0086   482 _U0CSR	=	0x0086
                     0087   483 _PCON	=	0x0087
                     0088   484 _TCON	=	0x0088
                     0089   485 _P0IFG	=	0x0089
                     008A   486 _P1IFG	=	0x008a
                     008B   487 _P2IFG	=	0x008b
                     008C   488 _PICTL	=	0x008c
                     008D   489 _P1IEN	=	0x008d
                     008E   490 __SFR8E	=	0x008e
                     008F   491 _P0INP	=	0x008f
                     0090   492 _P1	=	0x0090
                     0091   493 _RFIM	=	0x0091
                     0092   494 _DPS	=	0x0092
                     0093   495 _MPAGE	=	0x0093
                     0093   496 __XPAGE	=	0x0093
                     0094   497 __SFR94	=	0x0094
                     0095   498 __SFR95	=	0x0095
                     0096   499 __SFR96	=	0x0096
                     0097   500 __SFR97	=	0x0097
                     0098   501 _S0CON	=	0x0098
                     0099   502 __SFR99	=	0x0099
                     009A   503 _IEN2	=	0x009a
                     009B   504 _S1CON	=	0x009b
                     009C   505 _T2CT	=	0x009c
                     009D   506 _T2PR	=	0x009d
                     009E   507 _T2CTL	=	0x009e
                     009F   508 __SFR9F	=	0x009f
                     00A0   509 _P2	=	0x00a0
                     00A1   510 _WORIRQ	=	0x00a1
                     00A2   511 _WORCTRL	=	0x00a2
                     00A3   512 _WOREVT0	=	0x00a3
                     00A4   513 _WOREVT1	=	0x00a4
                     00A5   514 _WORTIME0	=	0x00a5
                     00A6   515 _WORTIME1	=	0x00a6
                     00A7   516 __SFRA7	=	0x00a7
                     00A8   517 _IEN0	=	0x00a8
                     00A9   518 _IP0	=	0x00a9
                     00AA   519 __SFRAA	=	0x00aa
                     00AB   520 _FWT	=	0x00ab
                     00AC   521 _FADDRL	=	0x00ac
                     00AD   522 _FADDRH	=	0x00ad
                     00AE   523 _FCTL	=	0x00ae
                     00AF   524 _FWDATA	=	0x00af
                     00B0   525 __SFRB0	=	0x00b0
                     00B1   526 _ENCDI	=	0x00b1
                     00B2   527 _ENCDO	=	0x00b2
                     00B3   528 _ENCCS	=	0x00b3
                     00B4   529 _ADCCON1	=	0x00b4
                     00B5   530 _ADCCON2	=	0x00b5
                     00B6   531 _ADCCON3	=	0x00b6
                     00B7   532 __SFRB7	=	0x00b7
                     00B8   533 _IEN1	=	0x00b8
                     00B9   534 _IP1	=	0x00b9
                     00BA   535 _ADCL	=	0x00ba
                     00BB   536 _ADCH	=	0x00bb
                     00BC   537 _RNDL	=	0x00bc
                     00BD   538 _RNDH	=	0x00bd
                     00BE   539 _SLEEP	=	0x00be
                     00BF   540 __SFRBF	=	0x00bf
                     00C0   541 _IRCON	=	0x00c0
                     00C1   542 _U0DBUF	=	0x00c1
                     00C2   543 _U0BAUD	=	0x00c2
                     00C3   544 __SFRC3	=	0x00c3
                     00C4   545 _U0UCR	=	0x00c4
                     00C5   546 _U0GCR	=	0x00c5
                     00C6   547 _CLKCON	=	0x00c6
                     00C7   548 _MEMCTR	=	0x00c7
                     00C8   549 __SFRC8	=	0x00c8
                     00C9   550 _WDCTL	=	0x00c9
                     00CA   551 _T3CNT	=	0x00ca
                     00CB   552 _T3CTL	=	0x00cb
                     00CC   553 _T3CCTL0	=	0x00cc
                     00CD   554 _T3CC0	=	0x00cd
                     00CE   555 _T3CCTL1	=	0x00ce
                     00CF   556 _T3CC1	=	0x00cf
                     00D0   557 _PSW	=	0x00d0
                     00D1   558 _DMAIRQ	=	0x00d1
                     00D2   559 _DMA1CFGL	=	0x00d2
                     00D3   560 _DMA1CFGH	=	0x00d3
                     00D4   561 _DMA0CFGL	=	0x00d4
                     00D5   562 _DMA0CFGH	=	0x00d5
                     00D6   563 _DMAARM	=	0x00d6
                     00D7   564 _DMAREQ	=	0x00d7
                     00D8   565 _TIMIF	=	0x00d8
                     00D9   566 _RFD	=	0x00d9
                     00DA   567 _T1CC0L	=	0x00da
                     00DB   568 _T1CC0H	=	0x00db
                     00DC   569 _T1CC1L	=	0x00dc
                     00DD   570 _T1CC1H	=	0x00dd
                     00DE   571 _T1CC2L	=	0x00de
                     00DF   572 _T1CC2H	=	0x00df
                     00E0   573 _ACC	=	0x00e0
                     00E1   574 _RFST	=	0x00e1
                     00E2   575 _T1CNTL	=	0x00e2
                     00E3   576 _T1CNTH	=	0x00e3
                     00E4   577 _T1CTL	=	0x00e4
                     00E5   578 _T1CCTL0	=	0x00e5
                     00E6   579 _T1CCTL1	=	0x00e6
                     00E7   580 _T1CCTL2	=	0x00e7
                     00E8   581 _IRCON2	=	0x00e8
                     00E9   582 _RFIF	=	0x00e9
                     00EA   583 _T4CNT	=	0x00ea
                     00EB   584 _T4CTL	=	0x00eb
                     00EC   585 _T4CCTL0	=	0x00ec
                     00ED   586 _T4CC0	=	0x00ed
                     00EE   587 _T4CCTL1	=	0x00ee
                     00EF   588 _T4CC1	=	0x00ef
                     00F0   589 _B	=	0x00f0
                     00F1   590 _PERCFG	=	0x00f1
                     00F2   591 _ADCCFG	=	0x00f2
                     00F3   592 _P0SEL	=	0x00f3
                     00F4   593 _P1SEL	=	0x00f4
                     00F5   594 _P2SEL	=	0x00f5
                     00F6   595 _P1INP	=	0x00f6
                     00F7   596 _P2INP	=	0x00f7
                     00F8   597 _U1CSR	=	0x00f8
                     00F9   598 _U1DBUF	=	0x00f9
                     00FA   599 _U1BAUD	=	0x00fa
                     00FB   600 _U1UCR	=	0x00fb
                     00FC   601 _U1GCR	=	0x00fc
                     00FD   602 _P0DIR	=	0x00fd
                     00FE   603 _P1DIR	=	0x00fe
                     00FF   604 _P2DIR	=	0x00ff
                            605 ;--------------------------------------------------------
                            606 ; special function bits
                            607 ;--------------------------------------------------------
                            608 	.area RSEG    (ABS,DATA)
   0000                     609 	.org 0x0000
                     0080   610 _P0_0	=	0x0080
                     0081   611 _P0_1	=	0x0081
                     0082   612 _P0_2	=	0x0082
                     0083   613 _P0_3	=	0x0083
                     0084   614 _P0_4	=	0x0084
                     0085   615 _P0_5	=	0x0085
                     0086   616 _P0_6	=	0x0086
                     0087   617 _P0_7	=	0x0087
                     0088   618 _IT0	=	0x0088
                     0089   619 _RFTXRXIF	=	0x0089
                     008A   620 _IT1	=	0x008a
                     008B   621 _URX0IF	=	0x008b
                     008D   622 _ADCIF	=	0x008d
                     008F   623 _URX1IF	=	0x008f
                     0090   624 _P1_0	=	0x0090
                     0091   625 _P1_1	=	0x0091
                     0092   626 _P1_2	=	0x0092
                     0093   627 _P1_3	=	0x0093
                     0094   628 _P1_4	=	0x0094
                     0095   629 _P1_5	=	0x0095
                     0096   630 _P1_6	=	0x0096
                     0097   631 _P1_7	=	0x0097
                     0098   632 _ENCIF_0	=	0x0098
                     0099   633 _ENCIF_1	=	0x0099
                     00A0   634 _P2_0	=	0x00a0
                     00A1   635 _P2_1	=	0x00a1
                     00A2   636 _P2_2	=	0x00a2
                     00A3   637 _P2_3	=	0x00a3
                     00A4   638 _P2_4	=	0x00a4
                     00A5   639 _P2_5	=	0x00a5
                     00A6   640 _P2_6	=	0x00a6
                     00A7   641 _P2_7	=	0x00a7
                     00A8   642 _RFTXRXIE	=	0x00a8
                     00A9   643 _ADCIE	=	0x00a9
                     00AA   644 _URX0IE	=	0x00aa
                     00AB   645 _URX1IE	=	0x00ab
                     00AC   646 _ENCIE	=	0x00ac
                     00AD   647 _STIE	=	0x00ad
                     00AF   648 _EA	=	0x00af
                     00B8   649 _DMAIE	=	0x00b8
                     00B9   650 _T1IE	=	0x00b9
                     00BA   651 _T2IE	=	0x00ba
                     00BB   652 _T3IE	=	0x00bb
                     00BC   653 _T4IE	=	0x00bc
                     00BD   654 _P0IE	=	0x00bd
                     00C0   655 _DMAIF	=	0x00c0
                     00C1   656 _T1IF	=	0x00c1
                     00C2   657 _T2IF	=	0x00c2
                     00C3   658 _T3IF	=	0x00c3
                     00C4   659 _T4IF	=	0x00c4
                     00C5   660 _P0IF	=	0x00c5
                     00C7   661 _STIF	=	0x00c7
                     00D0   662 _P	=	0x00d0
                     00D1   663 _F1	=	0x00d1
                     00D2   664 _OV	=	0x00d2
                     00D3   665 _RS0	=	0x00d3
                     00D4   666 _RS1	=	0x00d4
                     00D5   667 _F0	=	0x00d5
                     00D6   668 _AC	=	0x00d6
                     00D7   669 _CY	=	0x00d7
                     00D8   670 _T3OVFIF	=	0x00d8
                     00D9   671 _T3CH0IF	=	0x00d9
                     00DA   672 _T3CH1IF	=	0x00da
                     00DB   673 _T4OVFIF	=	0x00db
                     00DC   674 _T4CH0IF	=	0x00dc
                     00DD   675 _T4CH1IF	=	0x00dd
                     00DE   676 _OVFIM	=	0x00de
                     00E0   677 _ACC_0	=	0x00e0
                     00E1   678 _ACC_1	=	0x00e1
                     00E2   679 _ACC_2	=	0x00e2
                     00E3   680 _ACC_3	=	0x00e3
                     00E4   681 _ACC_4	=	0x00e4
                     00E5   682 _ACC_5	=	0x00e5
                     00E6   683 _ACC_6	=	0x00e6
                     00E7   684 _ACC_7	=	0x00e7
                     00E8   685 _P2IF	=	0x00e8
                     00E9   686 _UTX0IF	=	0x00e9
                     00EA   687 _UTX1IF	=	0x00ea
                     00EB   688 _P1IF	=	0x00eb
                     00EC   689 _WDTIF	=	0x00ec
                     00F0   690 _B_0	=	0x00f0
                     00F1   691 _B_1	=	0x00f1
                     00F2   692 _B_2	=	0x00f2
                     00F3   693 _B_3	=	0x00f3
                     00F4   694 _B_4	=	0x00f4
                     00F5   695 _B_5	=	0x00f5
                     00F6   696 _B_6	=	0x00f6
                     00F7   697 _B_7	=	0x00f7
                     00F8   698 _ACTIVE	=	0x00f8
                     00F9   699 _TX_BYTE	=	0x00f9
                     00FA   700 _RX_BYTE	=	0x00fa
                     00FB   701 _ERR	=	0x00fb
                     00FC   702 _FE	=	0x00fc
                     00FD   703 _SLAVE	=	0x00fd
                     00FE   704 _RE	=	0x00fe
                     00FF   705 _MODE	=	0x00ff
                     00E8   706 _USBIF	=	0x00e8
                            707 ;--------------------------------------------------------
                            708 ; overlayable register banks
                            709 ;--------------------------------------------------------
                            710 	.area REG_BANK_0	(REL,OVR,DATA)
   0000                     711 	.ds 8
                            712 ;--------------------------------------------------------
                            713 ; internal ram data
                            714 ;--------------------------------------------------------
                            715 	.area DSEG    (DATA)
                            716 ;--------------------------------------------------------
                            717 ; overlayable items in internal ram 
                            718 ;--------------------------------------------------------
                            719 ;--------------------------------------------------------
                            720 ; indirectly addressable internal ram data
                            721 ;--------------------------------------------------------
                            722 	.area ISEG    (DATA)
                            723 ;--------------------------------------------------------
                            724 ; absolute internal ram data
                            725 ;--------------------------------------------------------
                            726 	.area IABS    (ABS,DATA)
                            727 	.area IABS    (ABS,DATA)
                            728 ;--------------------------------------------------------
                            729 ; bit data
                            730 ;--------------------------------------------------------
                            731 	.area BSEG    (BIT)
                            732 ;--------------------------------------------------------
                            733 ; paged external ram data
                            734 ;--------------------------------------------------------
                            735 	.area PSEG    (PAG,XDATA)
                            736 ;--------------------------------------------------------
                            737 ; external ram data
                            738 ;--------------------------------------------------------
                            739 	.area XSEG    (XDATA)
                     DF02   740 _MDMCTRL0H	=	0xdf02
                     DF00   741 _SYNC1	=	0xdf00
                     DF01   742 _SYNC0	=	0xdf01
                     DF02   743 _PKTLEN	=	0xdf02
                     DF03   744 _PKTCTRL1	=	0xdf03
                     DF04   745 _PKTCTRL0	=	0xdf04
                     DF05   746 _ADDR	=	0xdf05
                     DF06   747 _CHANNR	=	0xdf06
                     DF07   748 _FSCTRL1	=	0xdf07
                     DF08   749 _FSCTRL0	=	0xdf08
                     DF09   750 _FREQ2	=	0xdf09
                     DF0A   751 _FREQ1	=	0xdf0a
                     DF0B   752 _FREQ0	=	0xdf0b
                     DF0C   753 _MDMCFG4	=	0xdf0c
                     DF0D   754 _MDMCFG3	=	0xdf0d
                     DF0E   755 _MDMCFG2	=	0xdf0e
                     DF0F   756 _MDMCFG1	=	0xdf0f
                     DF10   757 _MDMCFG0	=	0xdf10
                     DF11   758 _DEVIATN	=	0xdf11
                     DF12   759 _MCSM2	=	0xdf12
                     DF13   760 _MCSM1	=	0xdf13
                     DF14   761 _MCSM0	=	0xdf14
                     DF15   762 _FOCCFG	=	0xdf15
                     DF16   763 _BSCFG	=	0xdf16
                     DF17   764 _AGCCTRL2	=	0xdf17
                     DF18   765 _AGCCTRL1	=	0xdf18
                     DF19   766 _AGCCTRL0	=	0xdf19
                     DF1A   767 _FREND1	=	0xdf1a
                     DF1B   768 _FREND0	=	0xdf1b
                     DF1C   769 _FSCAL3	=	0xdf1c
                     DF1D   770 _FSCAL2	=	0xdf1d
                     DF1E   771 _FSCAL1	=	0xdf1e
                     DF1F   772 _FSCAL0	=	0xdf1f
                     DF20   773 __XREGDF20	=	0xdf20
                     DF21   774 __XREGDF21	=	0xdf21
                     DF22   775 __XREGDF22	=	0xdf22
                     DF23   776 _TEST2	=	0xdf23
                     DF24   777 _TEST1	=	0xdf24
                     DF25   778 _TEST0	=	0xdf25
                     DF26   779 __XREGDF26	=	0xdf26
                     DF27   780 _PA_TABLE7	=	0xdf27
                     DF28   781 _PA_TABLE6	=	0xdf28
                     DF29   782 _PA_TABLE5	=	0xdf29
                     DF2A   783 _PA_TABLE4	=	0xdf2a
                     DF2B   784 _PA_TABLE3	=	0xdf2b
                     DF2C   785 _PA_TABLE2	=	0xdf2c
                     DF2D   786 _PA_TABLE1	=	0xdf2d
                     DF2E   787 _PA_TABLE0	=	0xdf2e
                     DF2F   788 _IOCFG2	=	0xdf2f
                     DF30   789 _IOCFG1	=	0xdf30
                     DF31   790 _IOCFG0	=	0xdf31
                     DF32   791 __XREGDF32	=	0xdf32
                     DF33   792 __XREGDF33	=	0xdf33
                     DF34   793 __XREGDF34	=	0xdf34
                     DF35   794 __XREGDF35	=	0xdf35
                     DF36   795 _PARTNUM	=	0xdf36
                     DF37   796 _VERSION	=	0xdf37
                     DF38   797 _FREQEST	=	0xdf38
                     DF39   798 _LQI	=	0xdf39
                     DF3A   799 _RSSI	=	0xdf3a
                     DF3B   800 _MARCSTATE	=	0xdf3b
                     DF3C   801 _PKTSTATUS	=	0xdf3c
                     DF3D   802 _VCO_VC_DAC	=	0xdf3d
                     DF40   803 _I2SCFG0	=	0xdf40
                     DF41   804 _I2SCFG1	=	0xdf41
                     DF42   805 _I2SDATL	=	0xdf42
                     DF43   806 _I2SDATH	=	0xdf43
                     DF44   807 _I2SWCNT	=	0xdf44
                     DF45   808 _I2SSTAT	=	0xdf45
                     DF46   809 _I2SCLKF0	=	0xdf46
                     DF47   810 _I2SCLKF1	=	0xdf47
                     DF48   811 _I2SCLKF2	=	0xdf48
                     DF80   812 __NA_P0	=	0xdf80
                     DF81   813 __NA_SP	=	0xdf81
                     DF82   814 __NA_DPL0	=	0xdf82
                     DF83   815 __NA_DPH0	=	0xdf83
                     DF84   816 __NA_DPL1	=	0xdf84
                     DF85   817 __NA_DPH1	=	0xdf85
                     DF86   818 _X_U0CSR	=	0xdf86
                     DF87   819 __NA_PCON	=	0xdf87
                     DF88   820 __NA_TCON	=	0xdf88
                     DF89   821 _X_P0IFG	=	0xdf89
                     DF8A   822 _X_P1IFG	=	0xdf8a
                     DF8B   823 _X_P2IFG	=	0xdf8b
                     DF8C   824 _X_PICTL	=	0xdf8c
                     DF8D   825 _X_P1IEN	=	0xdf8d
                     DF8E   826 __X_SFR8E	=	0xdf8e
                     DF8F   827 _X_P0INP	=	0xdf8f
                     DF90   828 __NA_P1	=	0xdf90
                     DF91   829 _X_RFIM	=	0xdf91
                     DF92   830 __NA_DPS	=	0xdf92
                     DF93   831 _X_MPAGE	=	0xdf93
                     DF94   832 __X_SFR94	=	0xdf94
                     DF95   833 __X_SFR95	=	0xdf95
                     DF96   834 __X_SFR96	=	0xdf96
                     DF97   835 __X_SFR97	=	0xdf97
                     DF98   836 __NA_S0CON	=	0xdf98
                     DF99   837 __X_SFR99	=	0xdf99
                     DF9A   838 __NA_IEN2	=	0xdf9a
                     DF9B   839 __NA_S1CON	=	0xdf9b
                     DF9C   840 _X_T2CT	=	0xdf9c
                     DF9D   841 _X_T2PR	=	0xdf9d
                     DF9E   842 _X_T2CTL	=	0xdf9e
                     DF9F   843 __X_SFR9F	=	0xdf9f
                     DFA0   844 __NA_P2	=	0xdfa0
                     DFA1   845 _X_WORIRQ	=	0xdfa1
                     DFA2   846 _X_WORCTRL	=	0xdfa2
                     DFA3   847 _X_WOREVT0	=	0xdfa3
                     DFA4   848 _X_WOREVT1	=	0xdfa4
                     DFA5   849 _X_WORTIME0	=	0xdfa5
                     DFA6   850 _X_WORTIME1	=	0xdfa6
                     DFA7   851 __X_SFRA7	=	0xdfa7
                     DFA8   852 __NA_IEN0	=	0xdfa8
                     DFA9   853 __NA_IP0	=	0xdfa9
                     DFAA   854 __X_SFRAA	=	0xdfaa
                     DFAB   855 _X_FWT	=	0xdfab
                     DFAC   856 _X_FADDRL	=	0xdfac
                     DFAD   857 _X_FADDRH	=	0xdfad
                     DFAE   858 _X_FCTL	=	0xdfae
                     DFAF   859 _X_FWDATA	=	0xdfaf
                     DFB0   860 __X_SFRB0	=	0xdfb0
                     DFB1   861 _X_ENCDI	=	0xdfb1
                     DFB2   862 _X_ENCDO	=	0xdfb2
                     DFB3   863 _X_ENCCS	=	0xdfb3
                     DFB4   864 _X_ADCCON1	=	0xdfb4
                     DFB5   865 _X_ADCCON2	=	0xdfb5
                     DFB6   866 _X_ADCCON3	=	0xdfb6
                     DFB7   867 __X_SFRB7	=	0xdfb7
                     DFB8   868 __NA_IEN1	=	0xdfb8
                     DFB9   869 __NA_IP1	=	0xdfb9
                     DFBA   870 _X_ADCL	=	0xdfba
                     DFBB   871 _X_ADCH	=	0xdfbb
                     DFBC   872 _X_RNDL	=	0xdfbc
                     DFBD   873 _X_RNDH	=	0xdfbd
                     DFBE   874 _X_SLEEP	=	0xdfbe
                     DFBF   875 __X_SFRBF	=	0xdfbf
                     DFC0   876 __NA_IRCON	=	0xdfc0
                     DFC1   877 _X_U0DBUF	=	0xdfc1
                     DFC2   878 _X_U0BAUD	=	0xdfc2
                     DFC3   879 __X_SFRC3	=	0xdfc3
                     DFC4   880 _X_U0UCR	=	0xdfc4
                     DFC5   881 _X_U0GCR	=	0xdfc5
                     DFC6   882 _X_CLKCON	=	0xdfc6
                     DFC7   883 _X_MEMCTR	=	0xdfc7
                     DFC8   884 __X_SFRC8	=	0xdfc8
                     DFC9   885 _X_WDCTL	=	0xdfc9
                     DFCA   886 _X_T3CNT	=	0xdfca
                     DFCB   887 _X_T3CTL	=	0xdfcb
                     DFCC   888 _X_T3CCTL0	=	0xdfcc
                     DFCD   889 _X_T3CC0	=	0xdfcd
                     DFCE   890 _X_T3CCTL1	=	0xdfce
                     DFCF   891 _X_T3CC1	=	0xdfcf
                     DFD0   892 __NA_PSW	=	0xdfd0
                     DFD1   893 _X_DMAIRQ	=	0xdfd1
                     DFD2   894 _X_DMA1CFGL	=	0xdfd2
                     DFD3   895 _X_DMA1CFGH	=	0xdfd3
                     DFD4   896 _X_DMA0CFGL	=	0xdfd4
                     DFD5   897 _X_DMA0CFGH	=	0xdfd5
                     DFD6   898 _X_DMAARM	=	0xdfd6
                     DFD7   899 _X_DMAREQ	=	0xdfd7
                     DFD8   900 _X_TIMIF	=	0xdfd8
                     DFD9   901 _X_RFD	=	0xdfd9
                     DFDA   902 _X_T1CC0L	=	0xdfda
                     DFDB   903 _X_T1CC0H	=	0xdfdb
                     DFDC   904 _X_T1CC1L	=	0xdfdc
                     DFDD   905 _X_T1CC1H	=	0xdfdd
                     DFDE   906 _X_T1CC2L	=	0xdfde
                     DFDF   907 _X_T1CC2H	=	0xdfdf
                     DFE0   908 __NA_ACC	=	0xdfe0
                     DFE1   909 _X_RFST	=	0xdfe1
                     DFE2   910 _X_T1CNTL	=	0xdfe2
                     DFE3   911 _X_T1CNTH	=	0xdfe3
                     DFE4   912 _X_T1CTL	=	0xdfe4
                     DFE5   913 _X_T1CCTL0	=	0xdfe5
                     DFE6   914 _X_T1CCTL1	=	0xdfe6
                     DFE7   915 _X_T1CCTL2	=	0xdfe7
                     DFE8   916 __NA_IRCON2	=	0xdfe8
                     DFE9   917 _X_RFIF	=	0xdfe9
                     DFEA   918 _X_T4CNT	=	0xdfea
                     DFEB   919 _X_T4CTL	=	0xdfeb
                     DFEC   920 _X_T4CCTL0	=	0xdfec
                     DFED   921 _X_T4CC0	=	0xdfed
                     DFEE   922 _X_T4CCTL1	=	0xdfee
                     DFEF   923 _X_T4CC1	=	0xdfef
                     DFF0   924 __NA_B	=	0xdff0
                     DFF1   925 _X_PERCFG	=	0xdff1
                     DFF2   926 _X_ADCCFG	=	0xdff2
                     DFF3   927 _X_P0SEL	=	0xdff3
                     DFF4   928 _X_P1SEL	=	0xdff4
                     DFF5   929 _X_P2SEL	=	0xdff5
                     DFF6   930 _X_P1INP	=	0xdff6
                     DFF7   931 _X_P2INP	=	0xdff7
                     DFF8   932 _X_U1CSR	=	0xdff8
                     DFF9   933 _X_U1DBUF	=	0xdff9
                     DFFA   934 _X_U1BAUD	=	0xdffa
                     DFFB   935 _X_U1UCR	=	0xdffb
                     DFFC   936 _X_U1GCR	=	0xdffc
                     DFFD   937 _X_P0DIR	=	0xdffd
                     DFFE   938 _X_P1DIR	=	0xdffe
                     DFFF   939 _X_P2DIR	=	0xdfff
                     DE00   940 _USBADDR	=	0xde00
                     DE01   941 _USBPOW	=	0xde01
                     DE02   942 _USBIIF	=	0xde02
                     DE04   943 _USBOIF	=	0xde04
                     DE06   944 _USBCIF	=	0xde06
                     DE07   945 _USBIIE	=	0xde07
                     DE09   946 _USBOIE	=	0xde09
                     DE0B   947 _USBCIE	=	0xde0b
                     DE0C   948 _USBFRML	=	0xde0c
                     DE0D   949 _USBFRMH	=	0xde0d
                     DE0E   950 _USBINDEX	=	0xde0e
                     DE10   951 _USBMAXI	=	0xde10
                     DE11   952 _USBCS0	=	0xde11
                     DE11   953 _USBCSIL	=	0xde11
                     DE12   954 _USBCSIH	=	0xde12
                     DE13   955 _USBMAXO	=	0xde13
                     DE14   956 _USBCSOL	=	0xde14
                     DE15   957 _USBCSOH	=	0xde15
                     DE16   958 _USBCNT0	=	0xde16
                     DE16   959 _USBCNTL	=	0xde16
                     DE17   960 _USBCNTH	=	0xde17
                     DE20   961 _USBF0	=	0xde20
                     DE22   962 _USBF1	=	0xde22
                     DE24   963 _USBF2	=	0xde24
                     DE26   964 _USBF3	=	0xde26
                     DE28   965 _USBF4	=	0xde28
                     DE2A   966 _USBF5	=	0xde2a
   F9AA                     967 _debugx_text_1_48:
   F9AA                     968 	.ds 2
   F9AC                     969 _debug_text_1_50:
   F9AC                     970 	.ds 2
   F9AE                     971 _debughex_num_1_52:
   F9AE                     972 	.ds 1
   F9AF                     973 _debughex16_num_1_54:
   F9AF                     974 	.ds 2
   F9B1                     975 _debughex32_num_1_56:
   F9B1                     976 	.ds 4
                            977 ;--------------------------------------------------------
                            978 ; absolute external ram data
                            979 ;--------------------------------------------------------
                            980 	.area XABS    (ABS,XDATA)
                            981 ;--------------------------------------------------------
                            982 ; external initialized ram data
                            983 ;--------------------------------------------------------
                            984 	.area XISEG   (XDATA)
                            985 	.area HOME    (CODE)
                            986 	.area GSINIT0 (CODE)
                            987 	.area GSINIT1 (CODE)
                            988 	.area GSINIT2 (CODE)
                            989 	.area GSINIT3 (CODE)
                            990 	.area GSINIT4 (CODE)
                            991 	.area GSINIT5 (CODE)
                            992 	.area GSINIT  (CODE)
                            993 	.area GSFINAL (CODE)
                            994 	.area CSEG    (CODE)
                            995 ;--------------------------------------------------------
                            996 ; global & static initialisations
                            997 ;--------------------------------------------------------
                            998 	.area HOME    (CODE)
                            999 	.area GSINIT  (CODE)
                           1000 	.area GSFINAL (CODE)
                           1001 	.area GSINIT  (CODE)
                           1002 ;--------------------------------------------------------
                           1003 ; Home
                           1004 ;--------------------------------------------------------
                           1005 	.area HOME    (CODE)
                           1006 	.area HOME    (CODE)
                           1007 ;--------------------------------------------------------
                           1008 ; code
                           1009 ;--------------------------------------------------------
                           1010 	.area CSEG    (CODE)
                           1011 ;------------------------------------------------------------
                           1012 ;Allocation info for local variables in function 'debugx'
                           1013 ;------------------------------------------------------------
                           1014 ;len                       Allocated to registers r4 r5 
                           1015 ;text                      Allocated with name '_debugx_text_1_48'
                           1016 ;ptr                       Allocated with name '_debugx_ptr_1_49'
                           1017 ;------------------------------------------------------------
                           1018 ;	chipcon_usbdebug.c:7: void debugx(__xdata u8* __xdata  text)
                           1019 ;	-----------------------------------------
                           1020 ;	 function debugx
                           1021 ;	-----------------------------------------
   21B7                    1022 _debugx:
                     0007  1023 	ar7 = 0x07
                     0006  1024 	ar6 = 0x06
                     0005  1025 	ar5 = 0x05
                     0004  1026 	ar4 = 0x04
                     0003  1027 	ar3 = 0x03
                     0002  1028 	ar2 = 0x02
                     0001  1029 	ar1 = 0x01
                     0000  1030 	ar0 = 0x00
   21B7 AF 83         [24] 1031 	mov	r7,dph
   21B9 E5 82         [12] 1032 	mov	a,dpl
   21BB 90 F9 AA      [24] 1033 	mov	dptr,#_debugx_text_1_48
   21BE F0            [24] 1034 	movx	@dptr,a
   21BF EF            [12] 1035 	mov	a,r7
   21C0 A3            [24] 1036 	inc	dptr
   21C1 F0            [24] 1037 	movx	@dptr,a
                           1038 ;	chipcon_usbdebug.c:10: __xdata u8* __xdata  ptr = text;
   21C2 90 F9 AA      [24] 1039 	mov	dptr,#_debugx_text_1_48
   21C5 E0            [24] 1040 	movx	a,@dptr
   21C6 FE            [12] 1041 	mov	r6,a
   21C7 A3            [24] 1042 	inc	dptr
   21C8 E0            [24] 1043 	movx	a,@dptr
   21C9 FF            [12] 1044 	mov	r7,a
                           1045 ;	chipcon_usbdebug.c:11: while (*ptr++ != 0)
   21CA 7C 00         [12] 1046 	mov	r4,#0x00
   21CC 7D 00         [12] 1047 	mov	r5,#0x00
   21CE 8E 02         [24] 1048 	mov	ar2,r6
   21D0 8F 03         [24] 1049 	mov	ar3,r7
   21D2                    1050 00101$:
   21D2 8A 82         [24] 1051 	mov	dpl,r2
   21D4 8B 83         [24] 1052 	mov	dph,r3
   21D6 E0            [24] 1053 	movx	a,@dptr
   21D7 F9            [12] 1054 	mov	r1,a
   21D8 A3            [24] 1055 	inc	dptr
   21D9 AA 82         [24] 1056 	mov	r2,dpl
   21DB AB 83         [24] 1057 	mov	r3,dph
   21DD E9            [12] 1058 	mov	a,r1
   21DE 60 07         [24] 1059 	jz	00103$
                           1060 ;	chipcon_usbdebug.c:12: len ++;
   21E0 0C            [12] 1061 	inc	r4
   21E1 BC 00 EE      [24] 1062 	cjne	r4,#0x00,00101$
   21E4 0D            [12] 1063 	inc	r5
   21E5 80 EB         [24] 1064 	sjmp	00101$
   21E7                    1065 00103$:
                           1066 ;	chipcon_usbdebug.c:13: txdata(0xfe, 0xf0, len, (__xdata u8*)text);
   21E7 75 37 F0      [24] 1067 	mov	_txdata_PARM_2,#0xF0
   21EA 8C 38         [24] 1068 	mov	_txdata_PARM_3,r4
   21EC 8D 39         [24] 1069 	mov	(_txdata_PARM_3 + 1),r5
   21EE 8E 3A         [24] 1070 	mov	_txdata_PARM_4,r6
   21F0 8F 3B         [24] 1071 	mov	(_txdata_PARM_4 + 1),r7
   21F2 75 82 FE      [24] 1072 	mov	dpl,#0xFE
   21F5 02 1C 70      [24] 1073 	ljmp	_txdata
                           1074 ;------------------------------------------------------------
                           1075 ;Allocation info for local variables in function 'debug'
                           1076 ;------------------------------------------------------------
                           1077 ;len                       Allocated to registers r4 r5 
                           1078 ;text                      Allocated with name '_debug_text_1_50'
                           1079 ;ptr                       Allocated with name '_debug_ptr_1_51'
                           1080 ;------------------------------------------------------------
                           1081 ;	chipcon_usbdebug.c:16: void debug(__code u8* __xdata  text)
                           1082 ;	-----------------------------------------
                           1083 ;	 function debug
                           1084 ;	-----------------------------------------
   21F8                    1085 _debug:
   21F8 AF 83         [24] 1086 	mov	r7,dph
   21FA E5 82         [12] 1087 	mov	a,dpl
   21FC 90 F9 AC      [24] 1088 	mov	dptr,#_debug_text_1_50
   21FF F0            [24] 1089 	movx	@dptr,a
   2200 EF            [12] 1090 	mov	a,r7
   2201 A3            [24] 1091 	inc	dptr
   2202 F0            [24] 1092 	movx	@dptr,a
                           1093 ;	chipcon_usbdebug.c:19: __code u8* __xdata  ptr = text;
   2203 90 F9 AC      [24] 1094 	mov	dptr,#_debug_text_1_50
   2206 E0            [24] 1095 	movx	a,@dptr
   2207 FE            [12] 1096 	mov	r6,a
   2208 A3            [24] 1097 	inc	dptr
   2209 E0            [24] 1098 	movx	a,@dptr
   220A FF            [12] 1099 	mov	r7,a
                           1100 ;	chipcon_usbdebug.c:20: while (*ptr++ != 0)
   220B 7C 00         [12] 1101 	mov	r4,#0x00
   220D 7D 00         [12] 1102 	mov	r5,#0x00
   220F 8E 02         [24] 1103 	mov	ar2,r6
   2211 8F 03         [24] 1104 	mov	ar3,r7
   2213                    1105 00101$:
   2213 8A 82         [24] 1106 	mov	dpl,r2
   2215 8B 83         [24] 1107 	mov	dph,r3
   2217 E4            [12] 1108 	clr	a
   2218 93            [24] 1109 	movc	a,@a+dptr
   2219 F9            [12] 1110 	mov	r1,a
   221A A3            [24] 1111 	inc	dptr
   221B AA 82         [24] 1112 	mov	r2,dpl
   221D AB 83         [24] 1113 	mov	r3,dph
   221F E9            [12] 1114 	mov	a,r1
   2220 60 07         [24] 1115 	jz	00103$
                           1116 ;	chipcon_usbdebug.c:21: len ++;
   2222 0C            [12] 1117 	inc	r4
   2223 BC 00 ED      [24] 1118 	cjne	r4,#0x00,00101$
   2226 0D            [12] 1119 	inc	r5
   2227 80 EA         [24] 1120 	sjmp	00101$
   2229                    1121 00103$:
                           1122 ;	chipcon_usbdebug.c:22: txdata(0xfe, 0xf0, len, (__xdata u8*)text);
   2229 8E 3A         [24] 1123 	mov	_txdata_PARM_4,r6
   222B 8F 3B         [24] 1124 	mov	(_txdata_PARM_4 + 1),r7
   222D 75 37 F0      [24] 1125 	mov	_txdata_PARM_2,#0xF0
   2230 8C 38         [24] 1126 	mov	_txdata_PARM_3,r4
   2232 8D 39         [24] 1127 	mov	(_txdata_PARM_3 + 1),r5
   2234 75 82 FE      [24] 1128 	mov	dpl,#0xFE
   2237 02 1C 70      [24] 1129 	ljmp	_txdata
                           1130 ;------------------------------------------------------------
                           1131 ;Allocation info for local variables in function 'debughex'
                           1132 ;------------------------------------------------------------
                           1133 ;num                       Allocated with name '_debughex_num_1_52'
                           1134 ;------------------------------------------------------------
                           1135 ;	chipcon_usbdebug.c:25: void debughex(__xdata u8 num)
                           1136 ;	-----------------------------------------
                           1137 ;	 function debughex
                           1138 ;	-----------------------------------------
   223A                    1139 _debughex:
   223A E5 82         [12] 1140 	mov	a,dpl
   223C 90 F9 AE      [24] 1141 	mov	dptr,#_debughex_num_1_52
   223F F0            [24] 1142 	movx	@dptr,a
                           1143 ;	chipcon_usbdebug.c:27: txdata(0xfe, DEBUG_CMD_HEX, 1, (__xdata u8*)&num);
   2240 75 3A AE      [24] 1144 	mov	_txdata_PARM_4,#_debughex_num_1_52
   2243 75 3B F9      [24] 1145 	mov	(_txdata_PARM_4 + 1),#(_debughex_num_1_52 >> 8)
   2246 75 37 F1      [24] 1146 	mov	_txdata_PARM_2,#0xF1
   2249 75 38 01      [24] 1147 	mov	_txdata_PARM_3,#0x01
   224C 75 39 00      [24] 1148 	mov	(_txdata_PARM_3 + 1),#0x00
   224F 75 82 FE      [24] 1149 	mov	dpl,#0xFE
   2252 02 1C 70      [24] 1150 	ljmp	_txdata
                           1151 ;------------------------------------------------------------
                           1152 ;Allocation info for local variables in function 'debughex16'
                           1153 ;------------------------------------------------------------
                           1154 ;num                       Allocated with name '_debughex16_num_1_54'
                           1155 ;------------------------------------------------------------
                           1156 ;	chipcon_usbdebug.c:30: void debughex16(__xdata u16 num)
                           1157 ;	-----------------------------------------
                           1158 ;	 function debughex16
                           1159 ;	-----------------------------------------
   2255                    1160 _debughex16:
   2255 AF 83         [24] 1161 	mov	r7,dph
   2257 E5 82         [12] 1162 	mov	a,dpl
   2259 90 F9 AF      [24] 1163 	mov	dptr,#_debughex16_num_1_54
   225C F0            [24] 1164 	movx	@dptr,a
   225D EF            [12] 1165 	mov	a,r7
   225E A3            [24] 1166 	inc	dptr
   225F F0            [24] 1167 	movx	@dptr,a
                           1168 ;	chipcon_usbdebug.c:32: txdata(0xfe, DEBUG_CMD_HEX16, 2, (__xdata u8*)&num);
   2260 75 3A AF      [24] 1169 	mov	_txdata_PARM_4,#_debughex16_num_1_54
   2263 75 3B F9      [24] 1170 	mov	(_txdata_PARM_4 + 1),#(_debughex16_num_1_54 >> 8)
   2266 75 37 F2      [24] 1171 	mov	_txdata_PARM_2,#0xF2
   2269 75 38 02      [24] 1172 	mov	_txdata_PARM_3,#0x02
   226C 75 39 00      [24] 1173 	mov	(_txdata_PARM_3 + 1),#0x00
   226F 75 82 FE      [24] 1174 	mov	dpl,#0xFE
   2272 02 1C 70      [24] 1175 	ljmp	_txdata
                           1176 ;------------------------------------------------------------
                           1177 ;Allocation info for local variables in function 'debughex32'
                           1178 ;------------------------------------------------------------
                           1179 ;num                       Allocated with name '_debughex32_num_1_56'
                           1180 ;------------------------------------------------------------
                           1181 ;	chipcon_usbdebug.c:35: void debughex32(__xdata u32 num)
                           1182 ;	-----------------------------------------
                           1183 ;	 function debughex32
                           1184 ;	-----------------------------------------
   2275                    1185 _debughex32:
   2275 AF 82         [24] 1186 	mov	r7,dpl
   2277 AE 83         [24] 1187 	mov	r6,dph
   2279 AD F0         [24] 1188 	mov	r5,b
   227B FC            [12] 1189 	mov	r4,a
   227C 90 F9 B1      [24] 1190 	mov	dptr,#_debughex32_num_1_56
   227F EF            [12] 1191 	mov	a,r7
   2280 F0            [24] 1192 	movx	@dptr,a
   2281 EE            [12] 1193 	mov	a,r6
   2282 A3            [24] 1194 	inc	dptr
   2283 F0            [24] 1195 	movx	@dptr,a
   2284 ED            [12] 1196 	mov	a,r5
   2285 A3            [24] 1197 	inc	dptr
   2286 F0            [24] 1198 	movx	@dptr,a
   2287 EC            [12] 1199 	mov	a,r4
   2288 A3            [24] 1200 	inc	dptr
   2289 F0            [24] 1201 	movx	@dptr,a
                           1202 ;	chipcon_usbdebug.c:37: txdata(0xfe, DEBUG_CMD_HEX32, 4, (__xdata u8*)&num);
   228A 75 3A B1      [24] 1203 	mov	_txdata_PARM_4,#_debughex32_num_1_56
   228D 75 3B F9      [24] 1204 	mov	(_txdata_PARM_4 + 1),#(_debughex32_num_1_56 >> 8)
   2290 75 37 F3      [24] 1205 	mov	_txdata_PARM_2,#0xF3
   2293 75 38 04      [24] 1206 	mov	_txdata_PARM_3,#0x04
   2296 75 39 00      [24] 1207 	mov	(_txdata_PARM_3 + 1),#0x00
   2299 75 82 FE      [24] 1208 	mov	dpl,#0xFE
   229C 02 1C 70      [24] 1209 	ljmp	_txdata
                           1210 	.area CSEG    (CODE)
                           1211 	.area CONST   (CODE)
                           1212 	.area XINIT   (CODE)
                           1213 	.area CABS    (ABS,CODE)
