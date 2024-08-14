# Measure discspeed

- [Measure discspeed](#measure-discspeed)
  - [Table](#table)
  - [copy_fastq_arkiv2](#copy_fastq_arkiv2)
  - [copy_fastq_instrtmp](#copy_fastq_instrtmp)
  - [setq_downsample_fastq_arkiv2](#setq_downsample_fastq_arkiv2)
  - [setq_downsample_fastq_instrtmp](#setq_downsample_fastq_instrtmp)

## Table

| disc     | filesize | task                           | date             | duration                  | duration_secs |
| -------- | -------- | ------------------------------ | ---------------- | ------------------------- | ------------- |
| arkiv2   | 35G      | copy_fastq_arkiv2              | 2024_07_11_12_25 | 11 minutes and 22 seconds | NA            |
| arkiv2   | 35G      | copy_fastq_arkiv2              | 2024_07_11_13_21 | 10 minutes and 1 seconds  | NA            |
| arkiv2   | 35G      | copy_fastq_arkiv2              | 2024_07_11_14_55 | 9 minutes and 54 seconds  | NA            |
| arkiv2   | 35G      | copy_fastq_arkiv2              | 2024_07_11_16_40 | 9 minutes and 56 seconds  | 596           |
| arkiv2   | 35G      | copy_fastq_arkiv2              | 2024_08_13_11_37 | 10 minutes and 15 seconds | 615           |
| instrtmp | 35G      | copy_fastq_instrtmp            | 2024_07_11_13_23 | 1 minutes and 45 seconds  | NA            |
| instrtmp | 35G      | copy_fastq_instrtmp            | 2024_07_11_14_57 | 1 minutes and 45 seconds  | NA            |
| instrtmp | 35G      | copy_fastq_instrtmp            | 2024_07_11_16_41 | 1 minutes and 33 seconds  | 93            |
| instrtmp | 35G      | copy_fastq_instrtmp            | 2024_08_13_11_38 | 1 minutes and 43 seconds  | 103           |
| arkiv2   | 35G      | setq_downsample_fastq_arkiv2   | 2024_07_11_13_40 | 17 minutes and 27 seconds | NA            |
| arkiv2   | 35G      | setq_downsample_fastq_arkiv2   | 2024_07_11_15_14 | 17 minutes and 32 seconds | NA            |
| arkiv2   | 35G      | setq_downsample_fastq_arkiv2   | 2024_07_11_17_00 | 18 minutes and 10 seconds | 1090          |
| arkiv2   | 35G      | setq_downsample_fastq_arkiv2   | 2024_08_13_11_52 | 13 minutes and 12 seconds | 792           |
| instrtmp | 35G      | setq_downsample_fastq_instrtmp | 2024_07_11_14_19 | 11 minutes and 46 seconds | NA            |
| instrtmp | 35G      | setq_downsample_fastq_instrtmp | 2024_07_11_15_26 | 11 minutes and 49 seconds | NA            |
| instrtmp | 35G      | setq_downsample_fastq_instrtmp | 2024_08_13_12_04 | 11 minutes and 49 seconds | 709           |

## copy_fastq_arkiv2

    cp /mnt/Arkiv02/Execute_write_test_hal/fastq/12877_1_S3_R1_001.fastq.gz /mnt/Arkiv02/Execute_write_test_hal/Test3_copy

## copy_fastq_instrtmp

    sudo cp /mnt/InstrTemp/8_Bioinf/Halfdan_instTemp/Laboratoriemedicin/Precisions_medicinskt_laboratorium/Computational_resources/compare_disc_speeds/Execute_write_test_hal/fastq/12877_1_S3_R1_001.fastq.gz /mnt/InstrTemp/8_Bioinf/Halfdan_instTemp/Laboratoriemedicin/Precisions_medicinskt_laboratorium/Computational_resources/compare_disc_speeds/Execute_write_test_hal/Test3_copy

## setq_downsample_fastq_arkiv2

    /home/servicengs/bin/seqtk/seqtk sample -s100 /mnt/Arkiv02/Execute_write_test_hal/fastq/12877_1_S3_R1_001.fastq.gz 10000 > /mnt/Arkiv02/Execute_write_test_hal/Test1_downsampling/12877_1_S3_R1_001_10k.fastq.gz

## setq_downsample_fastq_instrtmp

    /home/servicengs/bin/seqtk/seqtk sample -s100 /mnt/InstrTemp/8_Bioinf/Halfdan_instTemp/Laboratoriemedicin/Precisions_medicinskt_laboratorium/Computational_resources/compare_disc_speeds/Execute_write_test_hal/fastq/12877_1_S3_R1_001.fastq.gz 10000 > /mnt/InstrTemp/8_Bioinf/Halfdan_instTemp/Laboratoriemedicin/Precisions_medicinskt_laboratorium/Computational_resources/compare_disc_speeds/Execute_write_test_hal/Test1_downsampling/12877_1_S3_R1_001.fastq_10k.gz
