
build: analyzer mmaping mprotecting bpf mprotect_perf_test mmap_perf_test read_char_device

clean:
	rm -f analyzer mmaping mprotecting bpf mprotect_perf_test mmap_perf_test read_char_device

analyzer: analyzer.c
	$(CC) -static -o $@ $< -I /usr/include/libnl3 -lnl-3 -lnl-genl-3

mmaping: mmaping.c
	$(CC) -o $@ $<

mprotecting: mprotecting.c
	$(CC) -o $@ $<

bpf: bpf_example.c
	$(CC) -o $@ $<

mprotect_perf_test: mprotect_perf_test.c
	$(CC) -o $@ $<

mmap_perf_test: mmap_perf_test.c
	$(CC) -o $@ $<

read_char_device: read_char_device.c
	$(CC) -o $@ $<