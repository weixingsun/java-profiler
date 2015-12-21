# lightweight java-profiler

java -agentpath:liblagent.so[:file=fname] [jvm flags]

#
src/globals.h:

// Number of times per second that we profile
static const int kNumInterrupts = 100;

// Maximum number of stack traces
static const int kMaxStackTraces = 3000;

// Maximum number of frames to store from the stack traces sampled.
static const int kMaxFramesToCapture = 128;
