zephyr_sources_if_kconfig(base64.c)

zephyr_sources(
  crc32_sw.c
  crc16_sw.c
  crc8_sw.c
  crc7_sw.c
  fdtable.c
  mempool.c
  rb.c
  thread_entry.c
  work_q.c
  )

zephyr_sources_ifdef(CONFIG_JSON_LIBRARY json.c)

zephyr_sources_if_kconfig(printk.c)

zephyr_sources_if_kconfig(ring_buffer.c)

zephyr_sources_ifdef(CONFIG_ASSERT assert.c)
