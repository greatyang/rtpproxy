TESTS = startstop basic_versions command_parser makeann extractaudio1 \
  session_timeouts playback1 forwarding1 rtp_analyze1 rtcp2json1 libucl1
startstop_EXTRA_DIST = startstop startstop.output
startstop_CLEANFILES = startstop.rout
basic_versions_EXTRA_DIST = basic_versions basic_versions.input basic_versions.output
basic_versions_CLEANFILES = basic_versions.qout basic_versions.rout
command_parser_EXTRA_DIST = command_parser command_parser.input command_parser.output
command_parser_CLEANFILES = command_parser.rout W3.IT2Nl*.rtcp W3.IT2Nl*.rtp \
  command_parser.rlog
extractaudio_EXTRA_DIST = extractaudio extractaudio1
extractaudio_CLEANFILES = *.mono.*.wav *.stereo.*.wav *.mono.*.wav.tout \
  *.stereo.*.wav.tout *.mono.*.raw *.mono.*.raw.tout *.mono.*.w64 \
  *.mono.*.w64.tout *.stereo.*.w64 *.stereo.*.w64.tout
playback1_EXTRA_DIST = playback1 playback1.output playback1.checksums \
  playback1.type1.input playback1.type2.input
playback1_CLEANFILES = playback1.0.a.rtp playback1.18.a.rtp playback1.3.a.rtp \
  playback1.8.a.rtp playback1.9.a.rtp playback1.0 playback1.18 playback1.3 \
  playback1.8 playback1.9 playback1.rout playback1.0.wav playback1.18.wav \
  playback1.3.wav playback1.8.wav playback1.9.wav playback1.tout playback1.rlog
forwarding1_EXTRA_DIST = forwarding1 forwarding1.checksums forwarding1.gen.input \
  forwarding1.gena.output forwarding1.geno.output forwarding1.input forwarding1.output \
  forwarding1.stats.input forwarding1.delete.input forwarding1.rec.input
forwarding1_CLEANFILES = forwarding1.0.wav forwarding1.18.wav forwarding1.3.wav \
  forwarding1.8.wav forwarding1.9.wav forwarding1.gena.rout forwarding1.geno.rout \
  forwarding1.rout forwarding1_[ao]_*.rtcp forwarding1_[ao]_*.rtp \
  forwarding1.0 forwarding1.3 forwarding1.8 forwarding1.9 forwarding1.18 \
  forwarding1.gena.rlog forwarding1.geno.rlog forwarding1.rlog
session_timeouts_EXTRA_DIST = session_timeouts session_timeouts.full.input \
  session_timeouts.full6.input session_timeouts.half.input \
  session_timeouts.half6.input session_timeouts.lookup.input \
  session_timeouts.lookup6.input session_timeouts.output1 session_timeouts.output2 \
  session_timeouts.stats.input session_timeouts6.output1 session_timeouts6.output2 \
  session_timeouts.tnotify.output
session_timeouts_CLEANFILES = session_timeouts.rout[1234] session_timeouts.rlog[1234] \
  session_timeouts.tlog session_timeouts.tlog.sorted session_timeouts.qout[1234] \
  session_timeouts.fout[1234]
rtp_analyze1_EXTRA_DIST = rtp_analyze1 rtp_analyze
rtp_analyze1_CLEANFILES = rtp_analyze_*.wav rtp_analyze_*.tout rtp_analyze_*.tlog
rtcp2json1_EXTRA_DIST = rtcp2json1 rtcp2json
rtcp2json1_CLEANFILES = rtcp1.output
libucl1_EXTRA_DIST = libucl1 libucl
libucl1_CLEANFILES = libucl_test.output
EXTRA_DIST = Makefile.am ${startstop_EXTRA_DIST} ${basic_versions_EXTRA_DIST} \
    ${command_parser_EXTRA_DIST} \
    ringback.sln makeann makeann.output \
    ${extractaudio_EXTRA_DIST} ${playback1_EXTRA_DIST} \
    ${forwarding1_EXTRA_DIST} ${session_timeouts_EXTRA_DIST} \
    ${rtp_analyze1_EXTRA_DIST} ${rtcp2json1_EXTRA_DIST} \
    ${libucl1_EXTRA_DIST}
# NB: AM_TESTS_ENVIRONMENT not available until automake 1.12
TESTS_ENVIRONMENT = \
        BASEDIR=${abs_srcdir} ; export BASEDIR ; \
        BUILDDIR=${abs_builddir} ; export BUILDDIR ; \
        TOP_BUILDDIR=${abs_top_builddir} ; export TOP_BUILDDIR ;
CLEANFILES = ringback.0 ringback.3 ringback.8 ringback.18 ringback.9 ${startstop_CLEANFILES} \
  ${extractaudio_CLEANFILES} ${playback1_CLEANFILES} ${forwarding1_CLEANFILES} \
  ${session_timeouts_CLEANFILES} ${command_parser_CLEANFILES} ${basic_versions_CLEANFILES} \
  ${rtp_analyze1_CLEANFILES} ${rtcp2json1_CLEANFILES} ${libucl1_CLEANFILES} *.core
