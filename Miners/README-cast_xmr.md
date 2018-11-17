~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

  Cast XMR 1.6.0 CryptoNight mining optimized for AMD Radeon Vega GPUs

  Coded by [glph3k] for more info visit http://www.gandalph3000.com
  Donating 1% mining power to developer. Thanks.

  For current stats press 's'
  For seamless exit press 'q'

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

```
Generic options:
  -h [ --help ]                 show this help message
  -O [ --opencl ] arg           index of the OpenCL plattform to use (-1 for
                                auto detect)
  -G [ --gpu ] arg (=0)         index of the GPUs to use. Separate by comma to
                                specify multiple GPUs e.g 0,1,2
  --log arg                     write to log file

Pool Configuration:
  -S [ --pool ] arg             pool server for a cryptonight based currency
  -u [ --user ] arg             user or wallet address for the pool
  -p [ --password ] arg         password for the pool server (if needed)
  --reconnects arg (=100)       pool reconnection attemps before quitting
  -a [ --algo ] arg (=-1)       hash algorithm to use: -1 for auto detect,
                                  0 = CryptoNight
                                  1 = CryptoNightV7
                                  2 = CryptoNight-Heavy
                                  3 = CryptoNight-Lite
                                  4 = CryptoNightV7-Lite
                                  5 = CryptoNightTUBE-Heavy
                                  6 = CryptoNightXTL
                                  7 = CryptoNightXHV-Heavy
                                  8 = CryptoNight-Fast
                                  9 = CryptoNightFEST
                                 10 = CryptoNightV8
  --nonicehash                  disable nicehasher support, use the full 32bit
                                nonce

Remote Access:
  -R [ --remoteaccess ]         enable remote access on 127.0.0.1:7777
  --remoteport arg (=7777)      set remote port to use

Optimizations:
  -I [ --intensity ] arg (=-1)  intensity levels. Separate by comma to specify
                                for each GPU. Range 0 to 10 (-1 = auto detect)
  --fastjobswitch               use fast job switching mode to prevent outdated
                                shares
  --ratewatchdog                enable watchdog on hash rate which resets a GPU
                                if necessary
```
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

YOU MUST DO THE FOLLOWING:

  1. Set "Miner name" to: cast_xmr
  2. Set "Installation URL" to: https://github.com/RevolutionRigs/hiveos/raw/master/Miners/cast_xmr-1.6.0.tar.gz
  3. In the "Extra config arguments" section add:
  3.1 Set --algo to a value 0-10 (currently only 0, 1, 10 are supported for stats): --algo 10
  3.2 Set --intensity to a value 1-10 for each GPU:                                 --intensity 10,10,10,10,10,10
  3.3 Set --gpu with a comma seperated list of all of your GPUs:                    --gpus 0,1,2,3,4,5

FINAL EXTRA CONFIG FOR 6 GPUs: --algo 10 --intensity 10,10,10,10,10,10 --gpus 0,1,2,3,4,5
